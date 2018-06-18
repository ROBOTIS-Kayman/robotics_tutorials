**Before you edit this code, Please make your own branch (ex, feature_xxx) or fork this repository to yours.**

Installation
===

```
$ sudo apt-get install ros-kinetic-gazebo-ros ros-kinetic-gazebo-ros-control
$ cakin_make
```

Run
===

```
$ roslaunch elfin_gazebo elfin3_empty_world.launch
```

Topics
===

```
/clock
/elfin3/joint1_position/command
/elfin3/joint2_position/command
/elfin3/joint3_position/command
/elfin3/joint4_position/command
/elfin3/joint5_position/command
/elfin3/joint6_position/command
/elfin3/joint_states
/gazebo/link_states
/gazebo/model_states
/gazebo/parameter_descriptions
/gazebo/parameter_updates
/gazebo/set_link_state
/gazebo/set_model_state
/rosout
/rosout_agg
```

Topic Info 
===

```
rostopic info /elfin3/joint1_position/command 
Type: std_msgs/Float64

Publishers: None

Subscribers: 
 * /gazebo (http://192.168.1.3:38072/)
```

Commands
===

```
$ rostopic pub /elfin3/joint1_position/command std_msgs/Float64 "data: 0.0" --once
```
