# omxplayersync

sudo apt-get update

sudo apt-get upgrade

su -
apt-get remove omxplayer

rm -rf /usr/bin/omxplayer /usr/bin/omxplayer.bin /usr/lib/omxplayer

wget -O- http://yokto.net/0/omxplayer/omxplayer-3176db4.tar.bz2 | tar -C / -xjvf -

ln -sf /lib/arm-linux-gnueabihf/libpcre.so.3 /lib/arm-linux-gnueabihf/libpcre.so.1

wget -O /usr/bin/omxplayer-sync https://github.com/turingmachine/omxplayer-sync/raw/master/omxplayer-sync

chmod 0755 /usr/bin/omxplayer-sync

wget https://github.com/turingmachine/omxplayer-sync/raw/master/synctest.mp4


sudo apt-get install python-setuptools

sudo easy_install pip

pip install pexpect

sudo apt-get install python-dbus


# start on master

omxplayer-sync -bmuv synctest.mp4


#force hdmi output

 hdmi_force_hotplug=1
 hdmi_drive=2
 
 #force audio out to rasp analog 3.5 jack
 
 sudo amixer cset numid=3 <output>

0=auto
1=headphones
2=hdmi

#disable screensaver

sudo apt-get install xscreensaver
