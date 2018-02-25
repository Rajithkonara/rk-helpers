---
layout: default
---
Reference:  <http://www.tecmint.com/mount-filesystem-in-linux/>

- Syntax
```sh
$ mount -t type device dir -o options
```
- Mounting a device with ro and noexec options
```sh
$ mount -t ext4 /dev/sdg1 /mnt -o ro,noexec
```
- Mounting NFS 
Reference: <http://www.tecmint.com/how-to-setup-nfs-server-in-linux/>

NFS servies

- portmap
- nfs
- rpc.mountd







