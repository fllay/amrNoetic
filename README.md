Rsapberry pi Buster 64bit download

https://downloads.raspberrypi.org/raspios_arm64/images/raspios_arm64-2021-05-28/

ROS Noetic installation

https://varhowto.com/install-ros-noetic-raspberry-pi-4/

It works only 64bit Buster not Bulleye.

Intsall packages  
```  
  sudo apt-get install -y python-rosdep python-rosinstall-generator python-wstool python-rosinstall build-essential cmake
  sudo apt install python-catkin-pkg
  sudo apt install ros-noetic-desktop
  sudo apt-get install -y python-rosdep python-rosinstall-generator python-wstool python-rosinstall build-essential cmake
  sudo apt-get install -y python-rosdep
  sudo apt install build-essential cmake
  sudo apt-get install ros-neotic-tf2-bullet
  sudo apt-get install ros-noetic-tf2-bullet
  sudo apt install ros-noetic-move-base-msgs
  sudo apt install libqt5serialport5
  sudo apt-get install ros-noetic-serial
  rosdep install
  sudo pip3 install libpython
  sudo apt install ros-noetic-rosserial
  sudo apt install libboost-all-dev 
  sudo apt install ros-noetic-geometry2
  sudo apt install ros-noetic-map-server
  sudo apt-get install ros-noetic-navigation
  sudo apt-get install ros-noetic-move-base-flex
  sudo apt-get install ros-noetic-teb-local-planner
  sudo apt install ros-noetic-teb-local-planner
  sudo apt install ros-noetic-tf2-geometry-msgs
  sudo apt install ros-noetic-rosbridge-suite
  sudo apt install ros-noetic-tf2-web-republisher
  sudo apt install ros-noetic-robot-localization
  sudo pip3 install rospy-message-converter
  sudo pip3 install parse_cmake
  sudo apt install libncurses5
  sudo apt-get install libudev-dev
```
Install node js
```
  sudo apt-get install -y nodejs
  npm install pm2 -g
  sudo npm install pm2 -g
```  
  
 
Install OpenCR firrmwaw

```git clone https://github.com/ROBOTIS-GIT/OpenCR.git```
 
 Make `opencr_ld` loader
 
```
 610  cd OpenCR/
  611  ls -l
  612  cd arduino/
  613  l s-0l
  614  ls -l
  615  cd opencr_develop/
  616  ls -l
  617  cd opencr_ld
  618  ls -l
  619  make
  620  ls -l
  621  ./opencr_ld
```

Stop ROS before download the firmware

```
pm2 stop 0
```
Download firmware and restart robot

```
./opencr_ld /dev/ttyACM0 115200 ./movebaseOprnCRwitMotion.ino.OpenCR.bin 
```
