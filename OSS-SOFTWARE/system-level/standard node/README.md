# Overview:
- Standard packages/software that should be present on every node
- System-Level environmental variables too
- Sun/Oracle Java JRE Version "1.8.0_191"

## Prerequisites (Tested on Ubuntu 16.04 Xenial):
- Preform the needed apt-get update
  * CLI Command:
    `sudo apt-get update`
- Create Directory Structure
  * /data/kickdatires/
  * /data/kickdatires/prod-software
  * CLI Command:
    `sudo mkdir -p -m 777 /opt/data/kick-da-tires/`
    `sudo mkdir -p -m 777 /opt/data/kick-da-tires/prod-software`

## Install Notes
- Tree
- VIM
- Pyhon 2.7.???
  *** Optional
- Python 3
- Sun/Oracle Java JRE Version "1.8.0_191"
  * Deflate TarBall
    * CLI Command:
      `sudo tar zxvf /data/kick-da-tires/INSTALLER/JRE-LATEST_jre-8u191-linux-x64.tar.gz -C /opt/data/kick-da-tires/prod-software`


In General:
sudo apt-get install tree vim vim-common vim-runtime gcc-5-base \
lib32stdc++6-5-dbg libjpeg-dev libxslt1-dev libxslt1.1 libunistring0 \
byobu libxml2  libgcc1 libstdc++6 binfmt-support lrzip cabextract

Python 2.X:
sudo apt-get install python python-tk python-doc python-tk python2.7-doc \
python-libxml2 python-libxslt1 python-pip

Python 3.X:
sudo apt-get install dh-python python3-lxml libpython3-stdlib \
libpython3.5 python3 python3-apport python3-cffi-backend \
python3-chardet python3-cryptography python3-dbus python3-debian \
python3-distupgrade python3-json-pointer python3-pkg-resources \
python3-prettytable python3-problem-report python3-serial python3-pip python3.5-doc\
python3-six python3-software-properties python3-yaml python3-doc

## Post Install:
- Set PATH to Java 1.8 as the default version
  * CLI Command:
    * export PATH=$PATH:/opt/data/kick-da-tires/prod-software/jre1.8.0_191/bin/
  * Manual Task:
    * Edit the "/etc/environment" file
      * Add to file
        * :/opt/data/kick-da-tires/prod-software/jre1.8.0_191/bin/

## Links:
- [GCC Home Page](https://gcc.gnu.org/ "GCC Home Page "GCC Home Page")
- [ttf-mscorefonts-installer Package Info](https://packages.ubuntu.com/xenial/ttf-mscorefonts-installer "Ubuntu 16.04 Xenial Package Info for ttf-mscorefonts-installer")
- [cabextract Package Info](https://packages.ubuntu.com/xenial/cabextract "Ubuntu 16.04 Xenial Package Info for cabextract")
