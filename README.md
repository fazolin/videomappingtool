# RASPIBERRY PI 3B+ SETUP GUIDE

- https://openframeworks.cc/setup/raspberrypi/raspberry-pi-getting-started/ (headless)
- v10 https://openframeworks.cc/versions/v0.10.1/of_v0.10.1_linuxarmv6l_release.tar.gz

#TRICK TO V10 ON BUSTER

I have OF up and running on my RPi 3 B using raspian Buster.

First, to install OF edit /home/pi/openFrameworks/scripts/linux/debian/install_dependencies.sh
change line 40 from:

apt-get install freeglut3-dev libasound2-dev libxmu-dev libxxf86vm-dev g++ libgl1-mesa-dev libglu1-mesa-dev libraw1394-dev libudev-dev libdrm-dev libglew-dev libopenal-dev libsndfile-dev libfreeimage-dev libcairo2-dev libfreetype6-dev libssl-dev libpulse-dev libusb-1.0-0-dev libgtk${GTK_VERSION}-dev libopencv-dev libegl1-mesa-dev libgles1-mesa-dev libgles2-mesa-dev libassimp-dev librtaudio-dev libboost-filesystem-dev libglfw3-dev  liburiparser-dev libcurl4-openssl-dev libpugixml-dev

to:

apt-get install freeglut3-dev libasound2-dev libxmu-dev libxxf86vm-dev g++ libgl1-mesa-dev libglu1-mesa-dev libraw1394-dev libudev-dev libdrm-dev libglew-dev libopenal-dev libsndfile-dev libfreeimage-dev libcairo2-dev libfreetype6-dev libssl-dev libpulse-dev libusb-1.0-0-dev libgtk${GTK_VERSION}-dev libopencv-dev libegl1-mesa-dev libglvnd-dev libassimp-dev librtaudio-dev libboost-filesystem-dev libglfw3-dev  liburiparser-dev libcurl4-openssl-dev libpugixml-dev

That allowed me to compile OF.

Then in my project config.make file I added on line 80:

PROJECT_LDFLAGS += -latomic 

I compiled and ran the polygon example!

# ofxPiMapper

- https://github.com/jvcleave/ofxOMXPlayer
- https://ofxpimapper.com/
- https://github.com/kr15h/ofxPiMapper
