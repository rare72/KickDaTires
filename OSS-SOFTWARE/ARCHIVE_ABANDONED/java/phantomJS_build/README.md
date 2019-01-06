# Overview:
- PhantomJS is utilized heavily build and compilation of OSS Java software. Listed below is how I utilize the software.
- Helps to properly setup the system for our usage.
  * Please remember to set the System-Wide $PATH to the location of this software.
- Integral Software that aids in the compilation of other OSS & system software.

## Prerequisites (Tested on Ubuntu 16.04 Xenial):
- cpp
  * The GNU C preprocessor is a macro processor that is used automatically by the GNU C compiler to transform programs before actual compilation.
    * cpp
- Python
  * interactive high-level object-oriented language (default python3 version)
  * Version 2.6 of higher
  * I challenged myself to compile this software with python 3
    * python3
    * python3-pip
    * python3-yaml
    * python3-fontconfig
    * python3-setuptools
    * python3-tk
    * python3-pkg-resources
- VIM
  * Vim is an almost compatible version of the UNIX editor Vi.
    * vim
- GNU C Library, C compilers & Other Compilers
  * GNU C Library + C Compilers
    * gcc
    * gcc-5
    * gcc-multilib
    * gcc-5-locales
    * libc6
    * libc-dev-bin
    * libc6-dev
    * libgcc-5-dev
    * g++
    * g++-multilib
    * g++-5-multilib
  * Other Compilers
    * gnu-standards
    * gfortran-5
    * libgfortran-5-dev
    * fortran95-compiler
- bison
  * Bison is a general-purpose parser generator
    * bison
- flex
  * Flex is a tool for generating scanners: programs which recognized lexical patterns in text.
    * flex
    * flex-doc
- libgoogle-perftools-dev
  * Perfect hash function generator
  * Also known as "gperf"
    * libgoogle-perftools-dev
- Perl
  * Larry Wall's Practical Extraction and Report Language
    * perl
- Ruby
  * Interpreter of object-oriented scripting language Ruby (default version)
    * ruby-all-dev
    * ruby-dev
    * ruby
- SQLite
  * SQLite 3 shared library
    * libsqlite3-dev
- FreeType
  * The FreeType project is a team of volunteers who develop free, portable and high-quality software solutions for digital typography.
    * libfreetype6
- OpenSSL
  * Secure Sockets Layer toolkit - development files
    * libssl-dev
- ICU
  * The International Components for Unicode (ICU)
    * libicu-dev
- gdb
  * GDB is a source-level debugger, capable of breaking programs at any specific line, displaying variable values, and determining where errors occurred.
    * gdb
  - libmpfr-dev
    * Multiple precision floating-point computation developers tools
      * libmpfr-dev
  - gettext
    * GNU Internationalization utilities
      * gettext
      * gettext-base
- make & Other supporting tools
  * make
    * utility for directing compilation
  * ~~make-guile~~
    * ~~utility for directing compilation with guile support~~
  * autoconf
    * The standard for FSF source packages.
  * automake
    * Tool for generating GNU Standards-compliant Makefiles
  * libtool
    * This is GNU libtool, a generic library support script.
  * manpages-dev
    * Manual pages about using GNU/Linux for development
  * update-notifier-common
    * Files shared between update-notifier and other packages
  * libmspack0
    * library for Microsoft compression formats (shared library)
  * install-info
    * Manage installed documentation in info format
### Java
  - gcj-jdk
    * gcj and Classpath development tools for Java(TM)
      * gcj-jdk


### System-Level Fonts
  - fonts-liberation
    * Fonts with the same metrics as Times, Arial and Courier
      * fonts-liberation
  - libfontenc1
    * X11 font encoding library
      * libfontenc-dev
      * libfontenc1
  - libxfont1
    * X11 font rasterisation library
      * libxfont1
      * libxfont1-dbg
      * libxfont1-dev
  - ~~x11-common~~
  - ~~xfonts-encodings~~
    * ~~Encodings for X.Org fonts~~
  - ~~xfonts-utils~~
    * ~~xfonts-utils provides a set of utility programs shipped with the X Window System that are needed for font management.~~
  - Fontconfig
    * Fontconfig (the package fontconfig or libfontconfig depending on the distribution)
    * Fontconfig is a font configuration and customization library, which does not depend on the X Window System.
      * fontconfig
      * fontconfig-config
      * libfontconfig1-dev
      * libfontconfig1
### Microsoft Fonts "ttf-mscorefonts-installer"
  - cabextract
    * *** Install this package first ***
    * This package is not found in the AWS repo's for Ubuntu 16.04 Xenial. You must download it manually.
  - ttf-mscorefonts-installer
    * This package allows for easy installation of the Microsoft True Type
    * This package is not found in the AWS repo's for Ubuntu 16.04 Xenial. You must download it manually.

## Install Software via Debian Based System
- CLI entries to install software  
    * Install the Various Prerequisites
      ```
      sudo apt-get install cpp python3 python3-pip python3-yaml python3-fontconfig python3-setuptools python3-tk python3-pkg-resources \
      vim gcc gcc-5 gcc-doc gcc-multilib g++ libc6 \
      libc-dev-bin libc6-dev libgcc-5-dev \
      bison flex flex-doc libgoogle-perftools-dev \
      perl ruby-all-dev ruby-dev ruby \
      libsqlite3-dev libfreetype6 libssl-dev libicu-dev \
      gdb make autoconf automake libtool manpages-dev update-notifier-common libmspack0 \
      fonts-liberation libfontenc-dev libfontenc1  libxfont1 libxfont1-dbg libxfont1-dev \
      fontconfig fontconfig-config libfontconfig1-dev libfontconfig1 \
      ```
    * Install the Microsoft Fonts
      ```
      sudo mkdir -p -m 777 /data/INSTALLER
      cd /data/INSTALLER; sudo wget http://mirrors.kernel.org/ubuntu/pool/multiverse/m/msttcorefonts/ttf-mscorefonts-installer_3.4+nmu1ubuntu2_all.deb
      cd /data/INSTALLER; sudo wget http://mirrors.kernel.org/ubuntu/pool/universe/c/cabextract/cabextract_1.6-1_amd64.deb
      cd /data/INSTALLER
      sudo apt install ./ttf-mscorefonts-installer_3.4+nmu1ubuntu2_all.deb
      sudo apt install ./cabextract_1.6-1_amd64.deb
      ```
## New Package Edition's
2108.12.15 @ 9:00pm

lib32stdc++6-5-dbg libx32stdc++6-5-dbg  autopoint libjpeg-dev qml-module-qtwebkit
python3-lxml libxslt1-dev libxslt1.1
python-libxslt1



libgcc1-dbg libgomp1-dbg libitm1-dbg libatomic1-dbg libasan2-dbg liblsan0-dbg libtsan0-dbg libubsan0-dbg libcilkrts5-dbg
libmpx0-dbg libquadmath0-dbg  

lib32stdc++6-5-dbg libx32stdc++6-5-dbg gfortran-5-multilib gfortran-5 libgfortran-5-dev libgfortran3 libgfortran3-dbg

libunistring0 libtinfo5 gettext-base libgomp1 libcroco3 libxml2

2018.12.16 @ 2:35am
PATH to python
PATH to gperf

sudo apt-get install python python-tk \
libc6 libgcc1 libqt5core5a libqt5gui5 libqt5network5 libqt5printsupport5 libqt5webkit5 \
libqt5widgets5 libstdc++6 libxrender-dev libxrender1 python-libxml2 python-leveldb \
gvfs cups-common libvisual-0.4-plugins gstreamer1.0-tools opus-tools libthai0 libqt5libqgtk2 qt5-image-formats-plugins qtwayland5 lm-sensors \
gstreamer1.0-plugins-base gvfs-backends libasound2-plugins alsa-utils librsvg2-common libjasper-runtime liblcms2-utils fancontrol sensord \
read-edid i2c-tools mesa-utils \
gvfs-backends libasound2-plugins alsa-utils librsvg2-common libjasper-runtime liblcms2-utils fancontrol sensord read-edid i2c-tools \
python-doc python-tk python2.7-doc binfmt-support mesa-utils \
blt-demo colord-sensor-argyll bluez-obexd samba-common libi2c-dev python-smbus lrzip libfftw3-bin libfftw3-dev libgd-tools gphoto2 \
libusbmuxd-tools jackd2 pulseaudio librsvg2-bin avahi-daemon hplip libsane-extras sane-utils tcl8.6 tk8.6 pinentry-doc python-examples tix \
python-tk-dbg rrdtool


- Failed Compile
Checking for fontconfig... yes
Checking for gccdepends... yes
Checking for glx... no
Checking for gnuld... yes
Checking for icu... yes
Checking for leveldb... no
Checking for libwebp... no
Checking for libXcomposite... no
Checking for libxml2... no
Checking for libXrender... no
Checking for libxslt... no
Checking for libzlib... yes

Encountered 5 configuration warning(s):

 ! QtQuick module not found, QML APIs will not be built
 ! Qt not configured to use system libjpeg, QImageDecoder will decode JPEG images
 ! Qt not configured to use system libpng, QImageDecoder will decode PNG images
 ! Missing GStreamer or QtMultimedia, disabling HTML5 media element support
 ! QtWebKitQml will not be build. It is not supported with static linking

The WebKit build was disabled for the following reasons:
    * Missing gperf from PATH
    * Missing python from PATH

Project ERROR: Unknown module(s) in QT: webkitwidgets

Possible New Packages:
python3-pyqt5.qtwebkit
python3-pyside.qtwebkit
webkit-image-qt
python-qt4 - Python bindings for Qt4
python-webkit - WebKit/Gtk Python bindings
python-webkit-dev

## Links:
- [PhantomJS Home Page](http://phantomjs.org "PhantomJS Home Page URL")
- [PhantomJS Download](http://phantomjs.org/download.html "PhantomJS Download URL")
- [PhantomJS Build](http://phantomjs.org/download.html "PhantomJS Build-Info URL")
- [GCC Home Page](https://gcc.gnu.org/ "GCC Home Page "GCC Home Page")
- [GPERF Home Page](http://code.google.com/p/gperftools/ "GPERF Home Page")
- [ttf-mscorefonts-installer Package Info](https://packages.ubuntu.com/xenial/ttf-mscorefonts-installer "Ubuntu 16.04 Xenial Package Info for ttf-mscorefonts-installer")
- [cabextract Package Info](https://packages.ubuntu.com/xenial/cabextract "Ubuntu 16.04 Xenial Package Info for cabextract")
