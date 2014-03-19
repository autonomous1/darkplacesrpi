darkplacesrpi
=============

Darkplaces Quake engine Raspberry PI version

Installation and configuration guide
====================================

<h3>Make sure system is up-to-date</h3>

sudo rpi-update

<h3>Create a folder somewhere for darkplaces</h3>

mkdir ~/darkplaces

cd ~/darkplaces

<h3>Download install package into folder</h3>

wget https://github.com/autonomous1/darkplacesrpi/archive/master.zip

<h3>Unpack and run installer</h3>

unzip -L -d ~/darkplaces master.zip

sudo dpkg -i darkplaces-rpi_1.0-0_all.deb

<h3>Download shareware version of Quake game data</h3>

wget ftp://ftp.idsoftware.com/idstuff/quake/quake106.zip

or select a faster mirror site to download quake106.zip:

http://linuxdocs.org/HOWTOs/Quake-HOWTO-2.html#quake-files

<h3>Unpack game data</h3>

unzip -L -d ~/darkplaces quake106.zip

sudo apt-get install lhasa

lhasa e resource.1

<h3>Setup user permissions</h3>

Note: replace pi with your username:

sudo usermod -a -G video pi

<h3>Run Darkplaces</h3>

darkplaces-sdl

(type esc for menu to start game or exit)

if you experience issues with no sound, keyboard or mouse input, try:

sudo darkplaces-sdl

<h3>Additional documentation</h3>

readme.darkplaces contains command line options, console commands and information on additional capabilities
