darkplacesrpi
=============

Darkplaces Quake engine Raspberry PI version

Installation and configuration guide
====================================

<h3>Make sure system is up-to-date</h3>

rpi-update

<h3>Create a folder for darkplaces:</h3>

mkdir ~/darkplaces

cd ~/darkplaces

<h3>Download shareware version of quake game data:</h3>

wget ftp://ftp.idsoftware.com/idstuff/quake/quake106.zip .

or select a mirror site to download quake106.zip:

http://linuxdocs.org/HOWTOs/Quake-HOWTO-2.html#quake-files

<h3>Unpack game data:</h3>

(a) install lha decompression tool:

sudo apt-get install lhasa

(b) unpack archive

unzip -L quake106.zip

lhasa e resource.1

<h3>Clone git project into directory:</h3>

git clone https://github.com/autonomous1/darkplacesrpi

<h3>Copy shared libraries to /usr/local/lib</h3>

sudo cp ./lib/* /usr/local/lib

<h3>Setup permissions</h3>

Note: replace pi with your username:

sudo usermod -a -G video pi

<h3>Run Darkplaces</h3>

./darkplaces

(type esc for menu to start game or exit)
