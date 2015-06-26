WebIOPi-0.7.1 Patch for Raspberry B+ and Pi 2
=============================================

You have full access to all header pins (40 pins) on the Web interface.

## Usage
------
$ tar xvzf WebIOPi-0.7.1.tar.gz  
$ cd WebIOPi-0.7.1  
$ wget https://raw.githubusercontent.com/doublebind/raspi/webiopi-pi2bplus.patch  
$ patch -p1 -i webiopi-pi2bplus.patch  
$ sudo ./setup.sh  
