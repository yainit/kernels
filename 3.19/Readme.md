		DERIVED FROM KERNEL 3.19 STANDARD AS OF LINUX FOUNDATION
====================================================================================

Find here the patches for the YaIniT 3.19 Kernel

The latest release is 3.19.7 

Patches for GNU Licensed Kernel find at  ftp.linux.org.tr or mirrors.
YAINIT (my patches, better adaption for GCC compilations and all logos)
UBUNTU (last version 17.17)
MAGEIA (incl. AUFS)
Fedora (most supplied patches)
GENTOO  (no PAX, no GRSECURITY)
OpenSuSE (here without XEN)
PCLinuxOS (some ports and corrections)
ZEN  (the Liquorix patch , BFS and other specialities)
BLD  (who absolutely wants to know it)
PUPPY (make the kernel absolutely compatible for Barry Kauler's earlier QUIRKY and PUPPY releases)
UKSM  (the Universalized Kernel Same page Merging)

Caution: This a test set, work in progress, and contains published patches from distributors. Nothing guaranteed! 


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

MP-TCP/TCP-Stealth was found to need to be always enabled, 
otherwise the compilation run exits with an error.


The used scripts for kernel generation follow in this directory and 
require an installed and working binary at /bin/busybox of your system


All modifications and adaptations by Dieter Miosga
dmiosga6200@gmail.com 
Please send mail with your bug description in case of failure
