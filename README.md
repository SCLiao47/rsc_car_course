# Prequest
## ROS Indigo
Please follow this [link](http://wiki.ros.org/indigo/Installation/Ubuntu) to install ROS Indigo.

## ROS Control
```
sudo apt-get install ros-indigo-ros-control ros-indigo-ros-controllers
```

## Serial Library
```
cd /tmp
git clone https://github.com/willie5588912/libserial-0.6.0rc2.git
cd libserial-0.6.0rc2
./configure
make
sudo make install
sudo ldconfig
```

