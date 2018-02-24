---
layout: default
---
- Finding files recursively according to the size
```sh
$ find . -maxdepth 3 -type f -size +2M
```
- find and delete files with user permission 777
```sh
$ find /home/user -perm 777 -exec rm '{}' + 
```