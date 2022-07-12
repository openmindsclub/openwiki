---
author: "Lilia Mehamli"
title: "Oracle 18c XE Installation Guide On Debian Based"
date: 2022-01-01
description: "Step by step guide to install Oracle 18c XE on Debian based hosts"
tags: ["oracle", "xe", "installation", "guide", "tutorial", "debian", "ubuntu", "mint"]
thumbnail: "/oracle-xe-installation-on-ubuntu/thumbnail.jpg"
---

## First Method

1. Download the three files 
   * `oracle-xe_11.2.0-1.0_amd64.debaa`
   * `oracle-xe_11.2.0-1.0_amd64.debab`
   *  `oracle-xe_11.2.0-1.0_amd64.debac`
  from [here](https://github.com/alexei-led/docker-oracle-xe-11g/tree/master/pkg)

2. Group them using `cat` like this
```bash
cat oracle-xe_11.2.0-1.0_amd64.deba* > oracle-xe_11.2.0-1.0_amd64.deb
```
Now you have a `.deb` file that you can install.

3. install the `.deb` file by doing:
```bash
sudo dpkg -i oracle-xe_11.2.0-1.0_amd64.deb
```
4. Configure your oracle thing by doing
 ```bash
sudo /etc/init.d/oracle-xe configure
```
 **ADVICE**: Don't activate the autolaunch thing.
* To launch it do :
```bash
sudo service oracle-xe start
```

### References:

* http://sampig.github.io/tutorial/2019/06/17/install-oracle-express-in-ubuntu

## Second Method

This should work with any distro/os that can run docker or a compatible docker software (podman for example)
Use docker , check [this link](https://hub.docker.com/r/oracleinanutshell/oracle-xe-11g)
