# docker-fsfreeze

[![CircleCI](https://circleci.com/gh/Intellection/docker-fsfreeze/tree/master.svg?style=svg&circle-token=61fff2811f0766a50f34853754ccd75bbe2d4ffd)](https://circleci.com/gh/Intellection/docker-fsfreeze/tree/master)

The [`fsfreeze`][1] command is used to suspend and resume access to a file system. This allows consistent snapshots to be taken by halting any new write system calls while allowing ongoing transactions to complete.

Supported filesystems:
* Ext3
* Ext4
* ReiserFS
* JFS
* XFS

Note: `fsfreeze` is unncessary for device-mapper devices. The device-mapper (and LVM) automatically freezes filesystem on the device when a snapshot creation is requested.

[1]: https://linux.die.net/man/8/fsfreeze
