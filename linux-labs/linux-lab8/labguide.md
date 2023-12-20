## Managing storage

### RAID and LVM
- Add 4 new disks on your VM (SCSI/SATA 5GB)
- List block devices, locate your new devices
- Configure a RAID1 with 2 of the disks. The recommended way now is to use LVM utility for both LVM and RAID (before lvm and mdadm tools where used)
  Identify 2 disks to group in RAID1.
- First look at partition tables on your main drive
- Check that no partition table exist on the 2 first drives that will be used (using parted for example
- Initialize the physical volumes and verify
- Create the volume group (VG) to aggregate the PV
- Create the RAID logical volume. Logical volumes are a way to partition a system as if they were traditional partitions but adding flexibility with the lvm abstraction layer.
- Check synchronization
- Scan block device again

### Filesystem
- Create file system (EXT4)
- Create a mount point and mount the volume
- Find out drive UUID to enable persistent mount
- Edit fstab
- Register new configuration and check mount points, then reboot

### Extend logical volume
- Check block device again
- Add a PV
- Add PV to the VG volgr1
- Extend the LV. Add 2G then take full available space
- Unmount FS, check volume and resize

### Journaling, inode
- Look for journaling option and inodes
- Check inode number
- Examine file information, find creation time
- Create a disk image using dd
- Examine journal information and recover a file using the sleuth kit (tsk)
