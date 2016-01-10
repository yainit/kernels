          PATCHES FOR KERNEL 4.3
=======================================================================

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

ANNOTATIONS:
============

The patches "Requiem for Ian Murdock" contain an unification of patches for 4.3.3 
from the distributions

Intel Clear Linux, OpenSuSE Tumbleweed-4.3.3-3.1, Mageia Cauldron, Gentoo,
Ubuntu-Xenial-5.16, PostFactum-PF and Liquorix-ZEN Fusion, Sunxi, PCLinuxOS,
TCP-Stealth TUM


The timely next patches ( As if they would have sentenced the GCC-Maintainer 
Jakub Jelinek for to walk forwards on the Santiago trail through Spain )
contain some more patches from Fedora-20, PCLinuxOS.
The speciality indeed is, that with the OpenSuSE-Tumbleweed32 Distribution as of 2015-12-21, 
the settings for AMD-k15 architecture compile to a working binary only with the old GCC-4.8 version.
With the GCC-5.2 version, the kernel crashes. Please feel free to use the toolchain switcher
that I wrote to change the symlinks for the current gcc-* commands from 5.2.1 to 4.8.3 and back. 
Find this in the toolchain/tools repository.



2016-01-10, 
Dieter Miosga 
 
