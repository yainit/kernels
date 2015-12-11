	DERIVED FROM KERNEL 3.19 STANDARD AS OF LINUX FOUNDATION ftp.kernel.org
====================================================================================

Find here the patches for the YaIniT 3.19 Kernel

The latest release is 3.19.8 

Contained therein are :
YAINIT (my patches, better adaption for GCC compilations and all logos)
UBUNTU (last version 17.17)
MAGEIA (incl. AUFS)
Fedora (most supplied patches)
GENTOO  (no PAX, no GRSECURITY)
OpenSuSE (here without XEN)
PCLinuxOS (some ports and corrections)
ZEN  (the Liquorix patch , BFS and other specialities)
BLD  (who absolutely wants to know it)
PUPPY (make the kernel absolutely compatible for Barry Kauler's QUIRKY and PUPPY releases)
UKSM  (the Universalized Kernel Same page Merging)
TCP-Stealth (the famous port knocker detection patch to avoid intrusions)

Caution: 
This a test set, work in progress, and contains published patches from distributors. 
Absolutely no warranty, nothing guaranteed! 


ANNOTATIONS:
============================================

For a kernel with configuration nearest to the kernel's make allmodconfig, 
are the modules packed in that squashfs file necessary,
that is generated with the do-makeg-ash or do-make-ash script to compile the kernel,   
to boot to a common marketed SDD/HDD connected to a widely marketed ATA/SATA controller.
Also you have to put this file into the initrd to load by the boot loader! 

If the drivers for the available disk drives are compiled in the kernel,
use the kernel commandline parameters    root=PARTUUID=    and    rootwait

If your boot device is /dev/sda3, than you get the PARTUUID by

linux:# fdisk -l /dev/sda|grep "Disk identifier:"|cut -f2 -d x

append -03 for the partition number and boot without initrd directly into your installed distro.

Preconfigured configurations are in the folder in files of type DOT.config-*

MP-TCP/TCP-Stealth was found to need to be always enabled, 
otherwise the compilation run exits with an error.


The used scripts for kernel generation follow in this directory and 
require an installed and working binary at /bin/busybox of your system


All modifications and adaptations by Dieter Miosga
dmiosga6200@gmail.com 
Please send mail with your bug description in case of failure
