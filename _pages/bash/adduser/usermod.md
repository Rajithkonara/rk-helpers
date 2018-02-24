---
layout: default
---
- expiary date to a account
```sh
$ usermod --expiredate 2017-10-30 rajith
```
- adding the user to supplementary group
```sh
$ usermod --append --groups root,users rajith
```
- changing default location of the home directory
```sh
$ usermod --home /tmp rajith
```
- changing the shell the user will by default
```sh
$ usermod --shell /bin/sh rajith
```