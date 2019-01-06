# Overview:
- PhantomJS is utilized heavily build and compilation of OSS Java software. Listed below is how I utilize the software.
- Helps to properly setup the system for our usage.
  * Please remember to set the System-Wide $PATH to the location of this software.
- Integral Software that aids in the compilation of other OSS & system software.

## Prerequisites (Tested on Ubuntu 16.04 Xenial):

## Install Notes
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
