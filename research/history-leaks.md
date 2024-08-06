## Quake Leaks

(Adapted from a [post to the forum](https://discuss.quaddicted.com/t/quake-alpha-version-from-1995/2593/92) on Quaddicted)

There are 3 real and distinct quake leaks:

1. 1996 Jun 11, Quake Beta v0.8 aka BETA3
2. 1996 Jun 22, Quake Pre-Release aka Press-Release
3. 1997 Jan 08, Linux Quake v1.01 Source Code

There may be more, but these were the ones I was able to corroborate with hard evidence.

If old quakers have heard whispers of more leaks, I'd love to hear about them.

**We don't endorse the leaks nor will I distribute them.** We need to know about their existence for the archive.



## Quake Beta v0.8 aka BETA3
* Filename like "q1prerelease.zip"
* md5sum: 64d7decd9445d2a1b0cd12bbedd1c1e4

readme snippet:

```text
+----------------------------------------+
| Quake BETA3 - not publicly released    |
| Tuesday, June 11th, 1996               |
| Copyright (C) 1996 id Software, inc.   |
+----------------------------------------+
```

archive content:

```text
    92726 29 Aug  1994 SETUP.EXE
    13787 29 Aug  1994 IPXSETUP.EXE
    20257 24 Dec  1994 SERSETUP.EXE
    15289 24 Feb  1996 SOUND.TXT
    11915 24 Feb  1996 VIDEO.TXT
    12018 24 Feb  1996 NETWORK.TXT
    25920 10 Jun  1996 CWSDPMI.EXE
    30034 10 Jun  1996 MANUAL.TXT
    12058 10 Jun  1996 README.TXT
    32256 10 Jun  1996 QUAKEUDP.DLL
    78848 10 Jun  1996 GENVXD.DLL
    10970 10 Jun  1996 MGENVXD.VXD
  1047040 10 Jun  1996 QLAUNCH.EXE
   358400 11 Jun  1996 QUAKE.EXE
      160 30 Jul 08:11 ID1
```

/id1:

```text
        24 10 Jun  1996 AUTOEXEC.CFG
  17204410 11 Jun  1996 PAK0.PAK
  29011451 11 Jun  1996 PAK1.PAK
```

* md5sum `quake.exe`: 4907286a331678ada634e535e0a2b41f
* md5sum `/id1/Pak0.pak:` 743ab1add442447848a9ad9f4ca4435f
* md5sum `/id1/Pak1.pak`: 3945725ec89ed1f6d16f2f47c106ef43

It runs fine in dosbox, v0.8 in console.

Running "version" command reports:

`exe: 23:09:18 june 10 1996`


It may have been leaked to `ftp.cdrom.com` with the filename `quakeb3.zip` and `quakeb-3.zip`, for example:


```text
ftp://ftp.cdrom.com/pub/idgames/incoming/quakeb-3.zip????

Steve Delorme
21 June 1996

ftp://ftp.cdrom.com/pub/idgames/incoming/quakeb-3.zip

could it be true?
```

-- [rec.games.computer.quake.misc](https://groups.google.com/g/rec.games.computer.quake.misc/c/deF4oQuT0R4/m/Ei0iZoZ4HUcJ)

People later in that thread claim to have downloaded and played it, referring to it by the name "BETA3".

Others found it to, for example [here](https://groups.google.com/g/tw.bbs.rec.pcgame/c/JTspV5KVm_8/m/y3I-GavIsfkJ), [here](https://groups.google.com/g/rec.games.computer.quake.misc/c/KbldZBFc_9E/m/vFiV-iZXOXsJ) and [here](https://groups.google.com/g/rec.games.computer.quake.misc/c/L4GGMZh1-1s/m/QodGXAXaxbgJ) (and more).



## Quake Pre-Release aka Press-Release
* Filename like "Pre-release quake.zip", or similar...
* md5sum: 815152d0de5a8f9010e1f20caa38db3c

readme snippet:

```text
+----------------------------------------+
| Quake PRE-RELEASE                      |
| Tuesday, June 11th, 1996               |
| Copyright (C) 1996 id Software, inc.   |
+----------------------------------------+
```

archive content:

```text
    15289 24 Feb  1996 Sound.txt
    11915 24 Feb  1996 Video.txt
    12018 24 Feb  1996 Network.txt
    25920 10 Jun  1996 Cwsdpmi.exe
    32256 10 Jun  1996 Quakeudp.dll
    78848 10 Jun  1996 Genvxd.dll
    10970 10 Jun  1996 Mgenvxd.vxd
  1047040 10 Jun  1996 Qlaunch.exe
       65 10 Jun  1996 Q95.bat
    12063 22 Jun  1996 Readme.txt
    30728 22 Jun  1996 Manual.txt
   358400 22 Jun  1996 Quake.exe
      192  7 Sep  2008 Id1
```

/id1:

```text
        24 10 Jun  1996 Autoexec.cfg
  29011451 11 Jun  1996 Pak1.pak
  17204410 22 Jun  1996 Pak0.pak
      2418 13 Apr  2009 Config.cfg
```

* md5sum `quake.exe`: 471a7fb830106929edd63d5ebcbb9f9b
* md5sum `id1/Pak0.pak`: f337fbe4656e2640c9aff35cb8db48a7
* md5sum `id1/Pak1.pak`: 3945725ec89ed1f6d16f2f47c106ef43 (same as above)

It runs in dosbox, no version in the console and console has no background image.

Running "version" command reports the same as above (different from file timestamp):

`exe: 23:09:18 june 10 1996`

## Quake v1.01 Source Code
* Filename like "quake101leakedsource.zip"
* md5sum: 3e1a412df05fc2fff7089e382bf33e7f


readme snippet:

```text
This is the infamous leak of the build 101 of Quake from iD, which contains an
initial port to Linux. This was 'liberated' from iD and ported to Linux on the
outside.
```

archive content:

```text
   1039 13 May  1992 rdpoint.asm
   1275 26 Jul  1996 xf86dga.c
    283 26 Jul  1996 cdaudio.h
    242 26 Jul  1996 cd_null.c
  17524 26 Jul  1996 cd_audio.c
   5231 26 Jul  1996 bspfile.h
   2059 26 Jul  1996 block8.h
   2110 26 Jul  1996 block16.h
   1793 26 Jul  1996 asm_i386.h
   3510 26 Jul  1996 asm_draw.h
   5565 26 Jul  1996 anorms.h
   9794 26 Jul  1996 adivtab.h
  21937 26 Jul  1996 d_draw16.s
  27408 26 Jul  1996 d_draw.s
   2610 26 Jul  1996 d_copy.s
   2658 26 Jul  1996 cvar.h
   3465 26 Jul  1996 cvar.c
    164 26 Jul  1996 crc.h
   2708 26 Jul  1996 crc.c
    710 26 Jul  1996 console.h
  10353 26 Jul  1996 console.c
   4586 26 Jul  1996 common.h
   3606 26 Jul  1996 cmd.h
  10828 26 Jul  1996 cmd.c
   7911 26 Jul  1996 client.h
   6580 26 Jul  1996 cl_tent.c
  18777 26 Jul  1996 cl_parse.c
  13789 26 Jul  1996 cl_main.c
  10243 26 Jul  1996 cl_input.c
   6019 26 Jul  1996 cl_demo.c
   2282 26 Jul  1996 modelgen.h
   7073 26 Jul  1996 model.h
  39112 26 Jul  1996 model.c
    358 26 Jul  1996 menu.h
   2078 26 Jul  1996 mathlib.h
   9157 26 Jul  1996 mathlib.c
   1686 26 Jul  1996 keys.h
  12655 26 Jul  1996 keys.c
   7723 26 Jul  1996 intercep.h
    283 26 Jul  1996 input.h
    186 26 Jul  1996 in_null.c
   7314 26 Jul  1996 in_dos.c
  28608 26 Jul  1996 host_cmd.c
  17310 26 Jul  1996 host.c
    685 26 Jul  1996 draw.h
   1703 26 Jul  1996 dosisms.h
   1193 26 Jul  1996 dosasm.s
   4113 26 Jul  1996 dos_v2.c
    131 26 Jul  1996 dmasim~3.c
   2049 26 Jul  1996 dmasim~1.c
   3147 26 Jul  1996 dmasim.c
    489 26 Jul  1996 d_zpoint.c
    782 26 Jul  1996 d_vars.c
  20492 26 Jul  1996 d_spr8.s
   2457 26 Jul  1996 d_sky.c
   1338 26 Jul  1996 d_scana.s
  10087 26 Jul  1996 d_scan.c
  23416 26 Jul  1996 d_polyse.c
   9230 26 Jul  1996 d_parta.s
   2957 26 Jul  1996 d_part.c
   1574 26 Jul  1996 d_modech.c
   2330 26 Jul  1996 d_local.h
   2634 26 Jul  1996 d_init.c
   2098 26 Jul  1996 d_ifacea.h
   5780 26 Jul  1996 d_iface.h
   1170 26 Jul  1996 d_fill.c
   6325 26 Jul  1996 r_aliasa.s
  17910 26 Jul  1996 r_alias.c
   4796 26 Jul  1996 r_aclipa.s
   7641 26 Jul  1996 r_aclip.c
    185 26 Jul  1996 quakeasm.h
   3909 26 Jul  1996 protocol.h
   3036 26 Jul  1996 progs.h
   2455 26 Jul  1996 progdefs.h
  11570 26 Jul  1996 pr_exec.c
  19439 26 Jul  1996 pr_edict.c
   2337 26 Jul  1996 pr_comp.h
  29602 26 Jul  1996 pr_cmds.c
    733 26 Jul  1996 nonintel.c
    951 26 Jul  1996 net_wins.h
   9798 26 Jul  1996 net_wins.c
   1212 26 Jul  1996 net_win.c
    560 26 Jul  1996 net_vcr.h
   2768 26 Jul  1996 net_vcr.c
    932 26 Jul  1996 net_udp.h
    563 26 Jul  1996 net_ser.h
  19666 26 Jul  1996 net_ser.c
    461 26 Jul  1996 net_none.c
    970 26 Jul  1996 net_mp.h
  10230 26 Jul  1996 net_mp.c
  17797 26 Jul  1996 net_main.c
    541 26 Jul  1996 net_loop.h
   4524 26 Jul  1996 net_loop.c
    932 26 Jul  1996 net_ipx.h
  17611 26 Jul  1996 net_ipx.c
   2247 26 Jul  1996 net_dos.c
    589 26 Jul  1996 net_dgrm.h
  29186 26 Jul  1996 net_dgrm.c
  27515 26 Jul  1996 net_comx.c
    913 26 Jul  1996 net_bw.h
  18156 26 Jul  1996 net_bw.c
   1167 26 Jul  1996 net_bsd.c
   9169 26 Jul  1996 net.h
  20041 26 Jul  1996 mplpc.c
   4759 26 Jul  1996 mplib.c
  26952 26 Jul  1996 mpdosock.h
  18970 26 Jul  1996 sys_dos.c
   1209 26 Jul  1996 sys.h
  10830 26 Jul  1996 sv_user.c
  25828 26 Jul  1996 sv_phys.c
   8585 26 Jul  1996 sv_move.c
  25647 26 Jul  1996 sv_main.c
  13247 26 Jul  1996 surf8.s
   2622 26 Jul  1996 surf16.s
   2078 26 Jul  1996 spritegn.h
   3864 26 Jul  1996 sound.h
   4207 26 Jul  1996 snd_win.c
    929 26 Jul  1996 snd_null.c
    684 26 Jul  1996 snd_next.c
   4128 26 Jul  1996 snd_mixa.s
  24099 26 Jul  1996 snd_gus.c
  12013 26 Jul  1996 snd_dos.c
  17549 26 Jul  1996 snd_dma.c
   5612 26 Jul  1996 server.h
    780 26 Jul  1996 screen.h
  17246 26 Jul  1996 screen.c
    534 26 Jul  1996 sbar.h
  17678 26 Jul  1996 sbar.c
    433 26 Jul  1996 resource.h
   3976 26 Jul  1996 render.h
    475 26 Jul  1996 r_vars.c
  13058 26 Jul  1996 r_surf.c
  10045 26 Jul  1996 r_sprite.c
   4416 26 Jul  1996 r_sky.c
   4007 26 Jul  1996 r_shared.h
  11840 26 Jul  1996 r_part.c
   8778 26 Jul  1996 r_misc.c
   7555 26 Jul  1996 r_local.h
   4590 26 Jul  1996 r_light.c
   4309 26 Jul  1996 r_efrag.c
  17144 26 Jul  1996 r_edgea.s
  14994 26 Jul  1996 r_edge.c
  18127 26 Jul  1996 r_drawa.s
  19373 26 Jul  1996 r_draw.c
  14113 26 Jul  1996 r_bsp.c
   2452 26 Jul  1996 zone.h
  17871 26 Jul  1996 zone.c
   1729 26 Jul  1996 world.h
  18682 26 Jul  1996 world.c
    112 26 Jul  1996 winquake.h
   1007 26 Jul  1996 wad.h
   2687 26 Jul  1996 wad.c
    649 26 Jul  1996 vregset.h
    978 26 Jul  1996 vregset.c
    163 26 Jul  1996 view.h
  19697 26 Jul  1996 view.c
   8766 26 Jul  1996 vid_vga.c
  12642 26 Jul  1996 vid_sv~1.c
  12137 26 Jul  1996 vid_op~1.c
   1245 26 Jul  1996 vid_null.c
  10500 26 Jul  1996 vid_ntgl.c
  37848 26 Jul  1996 vid_next.m
  18312 26 Jul  1996 vid_ext.c
   2086 26 Jul  1996 vid_dos.h
  13826 26 Jul  1996 vid_dos.c
   1904 26 Jul  1996 vid.h
  13831 26 Jul  1996 vgamodes.h
   4219 26 Jul  1996 sys_win.c
   7064 26 Jul  1996 sys_osf.c
   3000 26 Jul  1996 sys_null.c
   9624 26 Jul  1996 sys_next.m
    651 26 Jul  1996 sys_nexa.s
   7549 26 Jul  1996 sys_irix.c
   1242 26 Jul  1996 sys_dosa.s
   4891 27 Jul  1996 quakedef.h
   6746  2 Aug  1996 d_edge.c
   5953  2 Aug  1996 snd_mem.c
   9496  2 Aug  1996 d_sprite.c
   6223  5 Aug  1996 d_surf.c
  17790  5 Aug  1996 vid_x.c
  23556  5 Aug  1996 r_main.c
  58995  5 Aug  1996 menu.c
  15362  5 Aug  1996 draw.c
   8334  5 Aug  1996 snd_mix.c
  10012  5 Aug  1996 snd_aix.c
  15136  5 Aug  1996 vid_dfb.c
   8474  5 Aug  1996 sys_aix.c
   9388  5 Aug  1996 net_udp.c
   2681  5 Aug  1996 Makefile.bak
   2681  5 Aug  1996 Makefile
  16366  8 Aug  1996 vid_xf86.c
   2527  8 Aug  1996 readme~1.2
    182  8 Aug  1996 runme
   4705  9 Aug  1996 readme~1.3
   4704  9 Aug  1996 readme~1.4
   7777  9 Aug  1996 sys_linux.c
   4510 10 Aug  1996 snd_linux.c
     96 16 Jan  1997 intel_~1
    128 16 Jan  1997 alpha_~1
     96 16 Jan  1997 aix
  52342 19 Jan  1997 test
   4469 20 Jan  1997 dmasim~2.c
  44756 20 Jan  1997 d_polysa.s.orig
  44756 20 Jan  1997 d_polysa.s
  10588 20 Jan  1997 math.s.orig
  10588 20 Jan  1997 math.s
   2156 20 Jan  1997 worlda.s.bak
   2156 20 Jan  1997 worlda.s
   4469 20 Jan  1997 dmasim_linux.c
  31437 20 Jan  1997 common.c
```

A diff with the `WinQuake/` dir in the GPL'd `q1source.zip` release shows plausible regressions/differences in the c code.



