# ROS Cheatsheet

Launch Example 1: `roslaunch omx omx_testing.launch`

## ROS
### Running things
#### Executing Launch files
`roslaunch {PACKAGE} {FILE}.launch`

#### Running scripts
`rosrun {PACKAGE} {FILE}`
Note: if it fails to run, make sure the file is executable using `chmod +x {FILE}`

#### Run only master node
`roscore`

### Packages
#### Creating a new package
`catkin_create_pkg {NAME} rospy std_msgs {OTHER_DEPENDENCIES}`

#### Build packages
```
catkin build
src
```
### Topics 
#### List topics
`rostopic list`

#### Read messages from topic
`rostopic echo /{TOPIC}`

#### Publish message to topic
`rostopic pub /{TOPIC} {TYPE} {DATA}`

### Services
#### List services
`rosservice list`

#### Call service
`rosservice call /{SERVICE} {DATA}`

#### See service info
`rosservice info /{SERVICE}`

#### Get info about a message type
`rossrv info /{MESSAGE}`

### Other
#### See connections between nodes 
`rosrun rqt_graph rqt_graph`
## Using actual wafflebots
### Connecting
```bash
waffle 11 pair
waffle 11 term
roslaunch tuos_tb3_tools ros.launch # In the wafflebots terminal
```

### Shutdown

`waffle 11 off`
Then turn off at the switch when blue light disappears

## Environment setup
TODO: add info from old setup guide

## Troubleshooting
404 errors when installing packages: `sudo apt-get update` then try again
