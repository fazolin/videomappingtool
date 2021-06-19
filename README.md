# RASPIBERRY PI 3B SETUP GUIDE

- flash a SD car with http://downloads.raspberrypi.org/raspbian_lite/images/raspbian_lite-2019-04-09/
- cretae a ssh file in boot section to enable ssh on rpi
- folow https://github.com/openframeworks/ofSite/blob/4d1aa15a5a258f042f209619c9bf171adc1717c4/content/setup/raspberrypi/Raspberry-Pi-Getting-Started.md (of_v0.10.0)
- install git 
```
sudo apt install git
```
- clone https://github.com/jvcleave/ofxOMXPlayer into addons folder and folow instructions
- clone https://github.com/kr15h/ofxPiMapper into addons folder and folow instructions
- install node 

```
curl -fsSL https://deb.nodesource.com/setup_16.x | sudo -E bash -
sudo apt-get install -y nodejs
```
