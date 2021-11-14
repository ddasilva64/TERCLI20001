# File system

File System is responsible for storing information on disk and retrieving or updating

* Example : FAT32, NTFS

In Linux everything is file

**Types of File System**

* Network File System\
  NFS\
  SMB
* Disk File System\
  NTFS

**Network File System** are physically somewhere else, but appear as if they are mounted on one computer

* **NFS** -> was developed by Sun
* **SMB** -> was developed by Microsoft

**Physical structure on the disk**

| boot block                           | super block                         | block list |
| ------------------------------------ | ----------------------------------- | ---------- |
| information needs to boot the system | File System specifications size max | data file  |
|                                      |                                     |            |

**In operation, Linux kernel need to know**

* where data are stored
* how data can be accessed
* where we will save the new data

```
/
|
└─── bin
|
└─── opt
|
└─── boot
|
└─── root
|
└─── dev
|
└─── sbin
|
└─── etc
|
└─── srv
|
└─── home
|     └─── hannlecter
|     |     └─── work
|     |     └─── photos
|     └─── alien
|     └─── dvader
|
└─── tmp
|
└─── lib
|
└─── usr
|     └─── bin
|     └─── include
|     └─── lib
|     └─── sbin
|
└─── media
|
└─── var
|     └─── cache
|     └─── log
|     └─── spool
|     └─── tmp
|
└─── mnt
```

|           dir          | description                                                                                                                                                                                              |
| :--------------------: | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|            /           | the _**root filesystem**_ is the top-level directory. It must contain all of the files required to boot (include all of the required executables and libraries)                                          |
|          /bin          | contains user executable files                                                                                                                                                                           |
|          /opt          | optional files such as vendor supplied application programs                                                                                                                                              |
|          /boot         | contains files for booting the system                                                                                                                                                                    |
|          /dev          | contains the device files for hardware devices attached to the system (not device drivers, rather they are files that represent each device on the computer)                                             |
|          /sbin         | System Binary files. These are executables used for system administration                                                                                                                                |
|          /etc          | contains the local system configuration files for the host computer                                                                                                                                      |
|          /home         | storages for user files. Each user has a subdirectory home (f.e hannlecter, alien & dvader)                                                                                                              |
|          /tmp          | temporary directory. Used by the OS and many programs to store temporary files. Users may also store files here temporarily. Note that files stored here may be deleted at any time without prior notice |
|          /lib          | contains shared library files that are required to boot the system                                                                                                                                       |
|          /usr          | these are shareable, read-only files, including executable binaries and libraries, man files, and other types of documentation                                                                           |
|         /media         | a place to mount external removable media devices such as USB thumb drives that may be connected to the host                                                                                             |
|          /var          | variable data files are stored here. This can include things like log files, MySQL, and other database files, web server data files, email                                                               |
| inboxes, and much more |                                                                                                                                                                                                          |
|          /mnt          | a temporary mountpoint for regular filesystems (as in not removable media) that can be used while the administrator is repairing or working on a filesystem                                              |
|                        |                                                                                                                                                                                                          |
