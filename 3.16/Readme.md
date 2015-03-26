		DERIVED FROM KERNEL 3.16 STANDARD AS OF LINUX FOUNDATION
====================================================================================

Find here the patches for the YaIniT 3.16 Kernel

The latest release is 3.16.7 EndOfLife 
For now, only Canonical with its Ubuntu distribution makes priodically updates.

Please see the folder  ../libre-3.16-gnu for the patchset, which
includes modified patches from the following distributions or non-standard suppliers:

patch-3.16-gnu-3.16-7-gnu (original as of ftp.linux.org.tr)
YAINIT (my patches, better adaption for GCC compilations and all logos)
MAGEIA (incl. AUFS)
GENTOO  (no PAX, no GRSECURITY)
OpenSuSE (here without XEN)
PCLinuxOS (some ports and corrections)
ZEN  (the Liquorix patch , AUFS, BFQ, BFS and other specialities)
BLD  (who absolutely wants to know it)
PUPPY (make the kernel absolutely compatible for Barry Kauler's earlier QUIRKY and PUPPY releases)
MPTCP (Multipath TCP patch, allows better multi-connection management,
       port knocking and better intruder exclusion)
UKSM  (the Universalized Kernel Same page Merging)

Caution: This is a test sets and contains published patches from distributors. No Warranty! 


ANNOTATIONS:
============================================

For a kernel with configuration nearest allmodconfig are the modules necessary 
to boot to a common marketed SDD/HDD connected to a widely marketed ATA/SATA controller. 

If these drivres are compiled in the kernel,
use the kernel commandline parameters    root=PARTUUID=    and    rootwait

If your boot device is /dev/sda3, than you get the PARTUUID by

linux:# fdisk -l /dev/sda|grep "Disk identifier:"|cut -f2 -d x

append -03 for the partition number and boot without initrd directly into your installed distro.

Preconfigured configurations are in the folder in files of type DOT.config-*

MP-TCP was found to need to be always enabled, 
otherwise the compilation run exits with error.


The used scripts for kernel generation follow in this directory and 
require an installed and working binary at /bin/busybox of your system


All modifications and adaptations by Dieter Miosga
dmiosga6200@gmail.com 
Please send your mail with your bug description in case of failure
or with your intent for any colaboration

I do not welcome spam or whitnesses of Jehova, trying
to establish a world government by acts of religious activity
