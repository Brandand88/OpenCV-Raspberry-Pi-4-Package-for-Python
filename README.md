# OpenCV 4.5.0 For Raspberry Pi 3 and 4 Python 2 and 3

Raspbian Buster 10 Pre built OpenCV 4.5.0 
Turned on compile flags TBB NEON VFPV3

# Installation Step

wget https://github.com/cyysky/OpenCV-Raspberry-Pi-4-Package-for-Python/raw/master/opencv_4.5.0-1_armhf.deb

sudo dpkg -i opencv_4.5.0-1_armhf.deb       # This will install fail for dependency

sudo apt-get -f install                     # Auto install dependency package

sudo dpkg -i opencv_4.5.0-1_armhf.deb       # Now start install

#if have import issue https://github.com/EdjeElectronics/TensorFlow-Object-Detection-on-the-Raspberry-Pi/issues/67

export LD_PRELOAD=$LD_PRELOAD:/usr/lib/arm-linux-gnueabihf/libatomic.so.1.2.0

# Remove Step

sudo apt-get remove opencv

# Information
Check Raspberry Version
$ cat /etc/os-release
"Raspbian GNU/Linux 10 (buster)"

Installation guide mostly from
https://gist.github.com/willprice/abe456f5f74aa95d7e0bb81d5a710b60

https://www.learnopencv.com/install-opencv-4-on-raspberry-pi/

https://www.theimpossiblecode.com/blog/build-faster-opencv-raspberry-pi3/

https://www.pyimagesearch.com/2019/09/16/install-opencv-4-on-raspberry-pi-4-and-raspbian-buster/

http://www.codebind.com/linux-tutorials/install-opengl-ubuntu-linux/

http://www.makble.com/undefined-reference-to-glulookat-how-to-fix-in-mingw-on-windows


