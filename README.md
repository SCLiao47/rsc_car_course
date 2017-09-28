# Prequest
### Ubuntu 14.04
Please use [Ubuntu 14.04](http://releases.ubuntu.com/14.04/).

### ROS Indigo
Please follow this [link](http://wiki.ros.org/indigo/Installation/Ubuntu) to install ROS Indigo.

### ROS Control
```
sudo apt-get install ros-indigo-ros-control ros-indigo-ros-controllers
```

### Serial Library
```
cd /tmp
git clone https://github.com/willie5588912/libserial-0.6.0rc2.git
cd libserial-0.6.0rc2
./configure
make
sudo make install
sudo ldconfig
```
# Install
```
roscd; cd ../src
git clone https://github.com/willie5588912/rsc_car_course.git
cd ..
catkin_make
```
# Usage
## Real car
```
roslaunch rsc_car_ros_control rsc_car_ros_control.launch
```
Subscribe topic:
* /rsc_car_diff_drive_controller/cmd_vel

Publish topic:
* /rsc_car_diff_drive_controller/odom

So you can publish cmd_vel to control the car. For example, you can use rqt_robot_steering, using topic name **/rsc_car_diff_drive_controller/cmd_vel**
```
rosrun rqt_robot_steering rqt_robot_steering
```

## Simulation (optional)
```
roslaunch rsc_car_description rsc_car_gazebo.launch
```

