roach2_nfs_uboot
================

All files required to boot ROACH2 using NFS, u-boot, kernel and on rom file system

Untar debian file system as root to set correct permissions:
tar -xzvf snapshot_file

Check that symbolic links are correct in boot directory (to create symolic link: ln -s filename linkname):
"u-boot.bin" must point to required u-boot.bin file (e.g. u-boot-envfix.bin)
"romfs" must point to required romfs file (e.g. roach2-root-7.romfs)
"uImage" must point to required romfs file (e.g. uImage-r2borph3)