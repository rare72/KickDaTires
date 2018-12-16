# Overview:
#### PhantomJS is utilized heavily build and compilation of OSS Java software. Listed below is how I utilize the software.
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
- GNU C Library, C compiler & Standard GNU Software
  * GNU C Library
    * gcc
    * gcc-5
    * gcc-doc
    * gcc-multilib
    * g++
    * libc6
    * libc-dev-bin
    * libc6-dev
    * libgcc-5-dev
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
doc-base lib32stdc++6-5-dbg libx32stdc++6-5-dbg  autopoint
autoconf-archive gnu-standards  gettext   gcc-5-locales debian-keyring g++-multilib g++-5-multilib
libstdc++6-5-dbg libgcc1-dbg libgomp1-dbg libitm1-dbg libatomic1-dbg libasan2-dbg liblsan0-dbg libtsan0-dbg libubsan0-dbg libcilkrts5-dbg
libmpx0-dbg libquadmath0-dbg  |    libmpfr-dev  gfortran | fortran95-compiler gcj-jdk  ri bundler


## Links:
- [PhantomJS Home Page](http://phantomjs.org "PhantomJS Home Page URL")
- [PhantomJS Download](http://phantomjs.org/download.html "PhantomJS Download URL")
- [PhantomJS Build](http://phantomjs.org/download.html "PhantomJS Build-Info URL")
- [GCC Home Page](https://gcc.gnu.org/ "GCC Home Page "GCC Home Page")
- [GPERF Home Page](http://code.google.com/p/gperftools/ "GPERF Home Page")
- [ttf-mscorefonts-installer Package Info](https://packages.ubuntu.com/xenial/ttf-mscorefonts-installer "Ubuntu 16.04 Xenial Package Info for ttf-mscorefonts-installer")
- [cabextract Package Info](https://packages.ubuntu.com/xenial/cabextract "Ubuntu 16.04 Xenial Package Info for cabextract")
