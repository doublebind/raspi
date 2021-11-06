WebIOPi-0.7.1 Patch for Raspberry B+, Pi2, Pi3, and Pi4
=============================================

You have full access to all header pins (40 pins) on the Web interface.

既存のパッチに加えてBCM2711を搭載しているモデルでの問題を修正しています．
(Fixed a issue that prevented BCM2711 models (Raspberry Pi 4B) from passing the startup check.)

## Usage
------
$ wget http://sourceforge.net/projects/webiopi/files/WebIOPi-0.7.1.tar.gz  
$ tar xvzf WebIOPi-0.7.1.tar.gz  
$ cd WebIOPi-0.7.1  
$ wget https://raw.githubusercontent.com/UshiTaro/WebIOPi-for-Raspberry-Pi-4B/master/webiopi-pi2bplus.patch
$ patch -p1 -i webiopi-pi2bplus.patch  
$ sudo ./setup.sh

### How to Start WebIOPi

> Follow the steps below if Raspbian is installed by NOOBS later than 1.4.2.  

$ cd /etc/systemd/system/  
$ sudo wget https://raw.githubusercontent.com/doublebind/raspi/master/webiopi.service  
$ sudo systemctl start webiopi  
$ sudo systemctl enable webiopi  
