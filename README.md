darkplacesrpi
=============

Darkplaces Quake engine Raspberry PI version

Installation and configuration guide
====================================

**Make sure system is up-to-date**

`sudo rpi-update`

**Create a folder somewhere for darkplaces**

`mkdir ~/darkplaces`

`cd ~/darkplaces`

**Download install package into folder**

`wget https://github.com/autonomous1/darkplacesrpi/archive/master.zip`

**Unpack and run installer**

`unzip master.zip`

`mv darkplacesrpi-master/* .`

`sudo dpkg -i darkplaces-rpi_1.0-0_all.deb`

**Download shareware version of Quake game data**

`wget ftp://ftp.idsoftware.com/idstuff/quake/quake106.zip`

or select a faster mirror site to download quake106.zip:

http://linuxdocs.org/HOWTOs/Quake-HOWTO-2.html#quake-files

**Unpack game data**

`unzip quake106.zip`

`sudo apt-get install lhasa`

`lhasa e resource.1`

**Setup user permissions**

Note: replace pi with your username:

`sudo usermod -a -G video pi`

**Run Darkplaces**

`darkplaces-sdl`

(type esc for menu to start game or exit)

if you experience issues with no sound, keyboard or mouse input, try:

`sudo darkplaces-sdl`

**Additional documentation**

https://github.com/autonomous1/darkplacesrpi/wiki
