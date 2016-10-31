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

The patchset "confidential-tribute-to-the-sake-of-americas-workingpoors" contain the last unified selection 
of patches for version 4.8.5 of linux kernel from the distributions

Gentoo, Intel ClearOS, Sunxi-next-4.8.0-rc5, Ubuntu-4.8.0_27.29, OpenSuSE-4.8.3-1.1, 
ZEN (4.8.4-2.patch with scheduler MUQSS and EXFAT), Parabola (patch-4.8.4-gnu-pck1.patch with TCP-Stealth and UKSM), 
Debian-4.8.4, Mageia-Cauldron 6 4.8.2-mga1, Fedora 25 4.8.2, and with yainit-patches


These patches were all integrated and successfully compiled by Slackware-14.2-x86_32 distribution
with a changed toolset for GCC-4.9.4 and BINTUILS-2.27.  Both published sample kernel versions for the 
generic-x86-SSSE3 architecture processors and the AMD-15h Bulldozer AVX and later architecture
were running stable on each an AMD-FX6100 and an older Intel Atom Dual Core. 
The kernels were running under the Slackware-14.2-x86_32 distribution and the OSS-Tumbleweed32 as of 2016-05-12.
However these are samples and not tested under all conditions and come without any guarantee. 


Please feel free to use the toolchain switcher
that I wrote to change the symlinks to your current gcc-* commands. 
Find this in the toolchain/tools repository.


2016-10-31, 

Dieter Miosga 
 
