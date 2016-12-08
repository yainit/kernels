          PATCHES FOR KERNEL 4.8
==================================================

This repository contains the folders with the
kernel patchsets chosen and written to make the 
YaIniT kernel work the nearest possible to its designed functionality.

The patchsets for the standard kernel as downloadable from 
ftp://ftp.kernel.org    and mirrors
are in the folders with main version name  ?.??

The patchsets for the GNU/Libre Kernel without all proprietary
firmware as downloadable from 
http://linux-libre.fsfla.org/pub/linux-libre/releases/     and     ftp://ftp.linux.org.tr 
are in the folders with the name libre-?.??-gnu

Also use the scripts deblob*  for generation of the GNU/Libre kernel.

ANNOTATIONS, CHANGES :
============================================

The patchset "cold-sweat-under-chloridic-sky" contains the last unified selection 
of patches for version 4.8.6 of linux kernel from the distributions, the
patchset "for-the-untrumped-trump-ass" contains the 4.8.7 full patchset
together with the Realtime patches in time to this year's SuperFullMoon. 
The patchset "4.8.12-anticipated-distorted-xmas-melodies" contains 
the 4.8.12 full patchset, this turn with scheduling by the brand new MuQSS 
and with important corrections. Applied first to the 3.19 kernel, the kernel must not
die after detection of missing instructions, if it is the yainit-kernel. 
According to my experiments, this is a
misleading information, the running processor has these instructions.  

Gentoo, Intel ClearOS for 4.8.7, Sunxi-next-4.8.0-rc5 and Xunlong's Orange PI Allwinner-H3 integration, 
Ubuntu-4.8.0_27.29, OpenSuSE-4.8.3-1.1/-4.8.6-2.1, 
ZEN (4.8.10-1.patch with scheduler MUQSS and EXFAT), Parabola (patch-4.8.6-gnu-pck1.patch with TCP-Stealth and UKSM), 
AUR rcn-libre-4.8.6-arm-v7, Debian-4.8.4, Mageia-Cauldron 6 4.8.7-mga1, Fedora 25 4.8.2, and with revised yainit-patches


These patches were all integrated and successfully compiled by Slackware-14.2-x86_32 distribution
with a changed toolset to GCC-4.9.4 and BINTUILS-2.27.  Published sample kernel versions of 4.8.5 for the 
generic-x86-SSSE3 architecture processors and the AMD-15h Bulldozer AVX and later architecture
were running stable on each an AMD-FX6100 and an older Intel Atom Dual Core. 
The kernels were running under the Slackware-14.2-x86_32 distribution and the OSS-Tumbleweed32 as of 2016-05-12.
For the 4.8.6 is a generic i686 mostmod / nearest allmod version available.
However these are samples and not tested under all conditions and come without any guarantee. 


Please feel free to use the toolchain switcher
that I wrote to change the symlinks to your current gcc-* commands. 
Find this in the toolchain/tools repository.

--------------------------------------   I M P O R T A N T   -------------------------------------------------

During the revision of the patch runs, it appeared that a systematic inexactness or another Heisenbug in
the patch utility causes in some cases erroneous code with the potential
to produce involuntarily other Heisenbugs to the kernel WITHOUT ANY WARNING! 
To provide an ad-hoc solution to make apparent the real behaviour and the needs
of applied patches for modification, I added two separate patch utilities:


apply-patchesbbhard-ash


apply-patcheshard-ash


apply-patchessoft-ash 


The first one uses only the BusyBox applet patch, This allows no fuzzyness
for applying patches. To see the differences and possible failures, ot is recommended 
separately install the GNU-patch command 
The second hard patcher script will fall back to BusyBox patch if no other patch command available on your system. 
Anyway, there is the Fuzzyness parameter set to Zero!
The third and soft patcher script admits a fuzzyness of 120 and can be applied after the
first ones to catch and evaluate possible rejections. For the soft patcher script, there is no
fallback to or use of BusyBox instead  possible. 

------------------------------------------------------------------------------------------------------------------

2016-11-24, 

Dieter Miosga 
 
