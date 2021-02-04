File Systems
============

FAT(16) - file allocation table
FAT32
NTFS
EXT4
ZFS


Parity

* [Filesystem error handling](https://danluu.com/filesystem-errors/)
* [An Introduction to ZFS A Place to Start](https://www.servethehome.com/an-introduction-to-zfs-a-place-to-start/)
    * Block level snapshot restore
    * Raid-Z, Raid-Z2
    * Adaptive Replacement Cache

* [Reed-Solomon error recovery in RAID-6](https://anadoxin.org/blog/error-recovery-in-raid6.html/)

* [](https://twitter.com/jonasLyk/status/1347900440000811010)
    * > NTFS VULNERABILITY CRITICALITY UNDERESTIMATED
      > There is a specially nasty vulnerability in NTFS right now.
      > Triggerable by opening special crafted name in any folder anywhere.'
      > The vulnerability will instant pop up complaining about yuor harddrive is corrupted when path is opened
    * > The vulnerability can be remotely triggered if having any kind of service allowing file opens of specific names to happen.
      > Its embeddable in HTML, sharred folders etc. 
      >Until now only consequence have been running chkdsk on boot- but now the MFT have corrupted
    * > Its triggerable as a low privileged user- no special credentials or write permissions are needed.
    * > All that appears to be happening from this is that the volume dirty bits get flipped in the $Volume file.  Until those bits are reset, Windows will see the volume as corrupted.  The file system is not actually corrupted by .\:$i30:$bitmap.
    * > Seems like it can also be triggered when you paste the command in the URL of a browser except ie so far

didnt know where else to put this ...
* [tabfs](https://omar.website/tabfs/)
    * browser tabs (bi directional) as a filesystem mount
* [juicefs](https://github.com/juicedata/juicefs)
    * A distributed POSIX file system built on top of Redis and S3