# open_manipulator_X
(tested in Linux Ubuntu 20.04.6 LTS) 

## Installation

This repository contains Git Submodules which, upon cloning, creates empty package folders. These are submodules linking to [ROBOTIS-GIT](https://github.com/ROBOTIS-GIT).
To populate them, the following commands must be executed:
```
git submodule init
```
```
git submodule update
```
Additionally, some system packages are required for these submodules to function as expected:
```
sudo apt-get install ros-noetic-ros-controllers ros-noetic-gazebo* ros-noetic-moveit* ros-noetic-industrial-core
```
```
sudo apt install ros-noetic-dynamixel-sdk ros-noetic-dynamixel-workbench* ros-noetic-robotis-manipulator
```
To verify that your installation is functioning correctly, launch the omx_testing file to test the robot:
```
roslaunch omx omx_testing.launch
```
