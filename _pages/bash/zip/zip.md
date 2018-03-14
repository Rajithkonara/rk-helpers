---
layout: default
---

- Zip 
```sh
$ zip -r directory.zip directory
```
- Unzip 
```sh
$ unzip filename.zip
```
- TAR
```sh
$ tar -cvf directory.tar directory
```
- Create tar.gz
```sh
$ tar -cvzf directory.tar.gz directory
```
- UNTAR
```sh
$ tar -xvf directory.tar.gz
```
- List Content of tar Archive File
```sh
$ tar --tvf directory.tar.gz
```
- Untar Single file from tar File
```sh
$ tar -xvf product.v1.tar onefile.md
```
- Untar Single file from tar.gz File
```sh
$ tar -zxvf product.v1.tar onefile.md
```
- Options 
> c – Creates a new .tar archive file.

> v – Verbosely show the .tar file progress.

> f – File name type of the archive file.

> t – viewing content of archive file.

> j – filter archive through bzip2.

> z – filter archive through gzip.

> r – append or update files or directories to existing archive file.

> W – Verify a archive file.

> x – extract a archive file.