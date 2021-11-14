# Management of permissions and users



```
ls -l -> shows file permissions 
```

```bash
$ ls -l
drwxr-xr-x 1 Piotr 197609   0 Jul  9 16:43 'a.txt'
```

The permissions are shown in the first block of the result. In the example above it would be `drwxr-xr-x`.

Permissions can be separated as follows:

```
F/---/---/---
-: dir/link/file
---: owner (me) permissions
---: group permissions
---: everyone's permissions
```

**Mode type**

Permissions types:

* `r-–` -> read permission
* `rw-` -> read and write permission
* `rwx` -> read, write and execute permission

Permissions have numeric values:

* r = 4
* w = 2
* x = 1

| Owner | Group | World |
| :---: | :---: | :---: |
|  rwx  |  r-x  |  r-x  |
| 1 1 1 | 1 0 1 | 1 0 1 |
|       |       |       |

**Octal mode**

| Octal | Binary | Permissions |
| :---: | :----: | :---------: |
|   0   |   000  |     ---     |
|   1   |   001  |     --x     |
|   2   |   010  |     -w-     |
|   3   |   011  |     -wx     |
|   4   |   100  |     r--     |
|   5   |   101  |     r-x     |
|   6   |   110  |     rw-     |
|   7   |   111  |     rwx     |
|       |        |             |

| Owner | Group | World |
| :---: | :---: | :---: |
|  rwx  |  r-x  |  r-x  |
| 1 1 1 | 1 0 1 | 1 0 1 |
|   7   |   5   |   5   |
|       |       |       |

**Symbolic mode**

| Symbol | Meaning                              |
| :----: | ------------------------------------ |
|    u   | only for the user                    |
|    g   | only for the group                   |
|    o   | only for all others (it's the world) |
|    a   | applies to everyone                  |
|        |                                      |

```
chmod 755 myText             -> changes file permissions to 755
chmod u-r myText             -> removes file read permission
chmod u = rwx, go = r myText -> adds read, write, and run permissions to the user and only read to the group and others
id                           -> shows user ID
whoami                       -> shows name of logged in user
your userName                -> changes user
sudo command                 -> runs a command as superuser
```

To grant permissions we must give it a number that is the sum of each of these three letters:

```
---: 0
--x: 1
-r-: 2
-wx: 3
r--: 4
r-x: 5
rw-: 6
rwx: 7
```

To assign the permissions, the number must be given for both the owner, the group and the public.

```
---/---/---
666: rw-rw-rw-
750: rwxr-x---`
```

**Change permissions**

`chmod [number] <file>` -> allows you to change the permissions to a file

```bash
$ chmod 750 file.txt
```

**Run as super user**

```
sudo [script/command] -> run a command as super user
```
