# for linux blank screens


### edit this file

nano /etc/default/grub

### locate this line

GRUB_CMDLINE_LINUX_DEFAULT="quiet splash amd_iommu=off"


### for the freeze screen


GRUB_CMDLINE_LINUX_DEFAULT="quiet splash nouveau.modeset=0"