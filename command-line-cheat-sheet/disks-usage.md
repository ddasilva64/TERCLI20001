# Disks usage



```
df -h                                  -> shows free and used space on mounted systems
df -i                                  -> shows free inodes on mounted filesystems
fdisk -l                               -> shows disk partitions, sizes, and types
du -ah                                 -> shows disk usage for all files and directory
du -sh                                 -> shows disk usage of current directory
findmnt                                -> shows target mount point for all filesystems
mount [device_path] [mount_point]      -> mounts a device
```

The mount command mounts a storage device or filesystem, making it accessible and attaching it to an existing directory structure

```bash
$ mount -t type file-system mount-point
```

added a disk /dev/sdb on /data directory

```bash
$ mount -t ext4 /dev/sdb /data
```

The unmount command "unmounts" a mounted filesystem. Run unmount command with disk name or mount point name to unmount currently mounted disk

```bash
$ umount /dev/sdb
$ umount /data
```
