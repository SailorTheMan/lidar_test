# ROS workspace for unitree a1 slam.

## Installing
Install [unitree_ros_sdk](https://github.com/unitreerobotics/unitree_legged_sdk).
Install [cartographer](https://google-cartographer-ros.readthedocs.io/en/latest/compilation.html).
Install [Livox-SDK](https://github.com/Livox-SDK/Livox-SDK).

 `git clone https://github.com/SailorTheMan/lidar_test`
 `cd lidar_test`
 `catkin_make`

## Run sim

`roslaunch lidar_slam unitree_slam.launch`

## Run sim with bag file

`roslaunch lidar_slam unitree_bag.launch`</br>

## Run gazebo teleop:

    (optional) roslaunch unitree_gazebo normal.launch rname:=a1 
    rosrun unitree_controller unitree_move_teleop 
    rosrun teleop_twist_keyboard teleop_twist_keyboard.py 
