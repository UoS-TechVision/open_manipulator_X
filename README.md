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
sudo apt install ros-noetic-gazebo* ros-noetic-ros-control* ros-noetic-control* ros-noetic-moveit* ros-noetic-industrial-core
```
```
sudo apt install ros-noetic-dynamixel-sdk ros-noetic-dynamixel-workbench*
```
```
sudo apt install ros-noetic-robotis-manipulator
```
