

# Overview:
#### PhantomJS is utilized heavily build and compilation of OSS Java software. Listed below is how I utilize the software.
- Helps to properly setup the system for our usage.
  * Please remember to set the System-Wide $PATH to the location of this software.
- Integral Software that aids in the compilation of other OSS & system software.

## Prerequisites (Debian):
- cpp
  * The GNU C preprocessor is a macro processor that is used automatically by the GNU C compiler to transform programs before actual compilation.
    * cpp
- Python
  * interactive high-level object-oriented language (default python3 version)
  * Version 2.6 of higher
    * python3
    * python3-fontconfig
- VIM
  * Vim is an almost compatible version of the UNIX editor Vi.
    * vim
- GNU C Library & C compiler
  * GNU C Library GLIBCXX_3.4.9 "AND" GLIBC_2.7  
    * gcc
    * gcc-5
    * gcc-doc
    * gcc-multilib
    * g++
    * libc-dev-bin
    * libc6-dev
- bison
  * Bison is a general-purpose parser generator
    * bison
- flex
  * Flex is a tool for generating scanners: programs which recognized lexical patterns in text.
    * flex
    * flexc++
- gperf
  * Perfect hash function generator
    * gperf
- Perl
  * Larry Wall's Practical Extraction and Report Language
    * perl
- Ruby
  * Interpreter of object-oriented scripting language Ruby (default version)
    * ruby-build
    * ruby-qt4-dbg
    * ruby-all-dev
    * ruby-dev
    * ruby
- SQLite
  * SQLite 3 shared library
    * libsqlite3-dev
- FreeType
  * The FreeType project is a team of volunteers who develop free, portable and high-quality software solutions for digital typography.
    * libfreetype6
- Fontconfig
  * Fontconfig (the package fontconfig or libfontconfig depending on the distribution)
  * Fontconfig is a font configuration and customization library, which does not depend on the X Window System.
    * fontconfig
    * fontconfig-config
    * libfontconfig1-dev
    * libfontconfig1
- OpenSSL
  * Secure Sockets Layer toolkit - development files
    * libssl-dev
- ICU
  * The International Components for Unicode (ICU)
    * libicu-dev      Version: 57.1-6+deb9u2
- gdb
  * GDB is a source-level debugger, capable of breaking programs at any specific line, displaying variable values, and determining where errors occurred.
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
  * ttf-mscorefonts-installer
    * This package allows for easy installation of the Microsoft True Type

## Install Software via Debian Based System
- Command Line entry to deploy the software
    * ```
      sudo apt-get install build-essential g++ flex bison gperf perl \
      libsqlite3-dev libfontconfig1-dev libicu-dev libfreetype6 libssl-dev \
      libpng-dev libjpeg-dev libx11-dev libxext-dev \
      python3 python3-fontconfig cpp vim flexc++ \
      gcc gcc-5 gcc-doc gcc-multilib g++ libc-dev-bin libc6-dev \
      ruby-build ruby-qt4-dbg ruby-all-dev ruby-dev ruby \
      fontconfig fontconfig-config libfontconfig1-dev libfontconfig1 \
      gdb make make-guile autoconf automake libtool manpages-dev ttf-mscorefonts-installer
      ```

## Links:
- [Main Page](http://phantomjs.org "Main PhantomJS URL")
- [Download PhantomJS](http://phantomjs.org/download.html "PhantomJS Download URL")
- [GCC Home Page](https://gcc.gnu.org/ "GCC Main Home Page")
