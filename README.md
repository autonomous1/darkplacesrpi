darkplacesrpi
=============

Darkplaces Quake engine Raspberry PI version

Installation and configuration guide
====================================

1. Create a folder for darkplaces:

mkdir ~/darkplaces
cd ~/darkplaces

2. Download shareware version of quake game data:

wget ftp://ftp.idsoftware.com/idstuff/quake/quake106.zip .

or select a mirror site to download quake106.zip:
http://linuxdocs.org/HOWTOs/Quake-HOWTO-2.html#quake-files

3. Unpack game data:

(a) install lha decompression tool:
sudo apt-get install lhasa

(b) unpack archive
unzip -L quake106.zip
lhasa e resource.1

4. Clone git project into directory:

git clone https://github.com/autonomous1/darkplacesrpi

