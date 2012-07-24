roach2_nfs_uboot
================

All files required to boot ROACH2 using NFS, u-boot, kernel and on rom file system

These files usually go in "/home/nfs/roach2/", but this depends on how NFS and dnsmasq is configured. 
Please perform all action as ROOT to retain correct permissions (git clone as ROOT). 

Untar debian file system as ROOT to set correct permissions: tar -xzvf snapshot_file
Now create a symbolic link: ln -s debian-stable-devel current
When ROACH2 boots it will look for "current" in the NFS directory.

Check that symbolic links are correct in boot directory (to create symolic link: ln -s filename linkname):
"u-boot.bin" must point to required u-boot.bin file (e.g. u-boot-envfix.bin)
"romfs" must point to required romfs file (e.g. roach2-root-7.romfs)
"uImage" must point to required romfs file (e.g. uImage-r2borph3)