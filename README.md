WebIOPi-0.7.1 Patch for Raspberry B+ and Pi 2
=============================================

You have full access to all header pins (40 pins) on the Web interface.

## Usage
------
$ wget http://sourceforge.net/projects/webiopi/files/WebIOPi-0.7.1.tar.gz  
$ tar xvzf WebIOPi-0.7.1.tar.gz  
$ cd WebIOPi-0.7.1  
$ wget https://raw.githubusercontent.com/doublebind/raspi/master/webiopi-pi2bplus.patch  
$ patch -p1 -i webiopi-pi2bplus.patch  
$ sudo ./setup.sh

### How to Start WebIOPi

> Follow the steps below if Raspbian is installed by NOOBS later than 1.4.2.  

$ cd /etc/systems/system/  
$ sudo wget https://raw.githubusercontent.com/doublebind/raspi/master/webiopi.service  
$ sudo systemctl start webiopi  
$ sudo systemctl enable webiopi  
