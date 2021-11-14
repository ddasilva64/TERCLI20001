# Hardware information



```
dmesg                    -> shows bootup messages
cat /proc/cpuinfo        -> shows CPU information 
free -h                  -> shows free and used memory (-m flag indicates memory in MB)
lshw                     -> lists information about hardware configuration
lsblk                    -> lists information about block devices
lspci -tv                -> shows PCI devices in a tree-like diagram 
lsusb -tv                -> shows USB devices in a tree-like diagram
dmidecode                -> shows hardware information from the BIOS
hdparm -i /dev/[disk]    -> shows information about disk data
hdparm -tT /dev/[disk]   -> conducts a read speed test on disk
badblocks -s /dev/[disk] -> tests for unreadable blocks on disk
```
