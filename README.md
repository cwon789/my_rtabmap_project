# my_rtabmap_project

1. PRE-Installed
 - RTAB-MAP, RTAB-MAP_ROS 
  - sudo apt-get install ros-melodic-rtabmap
  - sudo apt-get install ros-melodic-ratbmap-ros
 - Realsense_ros https://github.com/IntelRealSense/realsense-ros.git
 - turtlebot_bringupwith_rplidar https://github.com/cwon789/turtlbot_bringupwith_rplidar.git

2. Put these launch files in your workspace. In my case, the path is catkin_ws2/src/realsense-ros/realsense2_camera/launch

3. Launch these files
 - roslaunch turtlebot3_bringup turtlebot3_core_rplidar.launch   ---->   turtlebot3 node 
 - roslaunch realsense2_camera rs_camera.launch     ---->    realsnese d435i node
 - roslaunch realsense2_camera opensource_tracking2.launch     ---->    rtabmap
 
#####
4. additional 
 -  roslaunch explore_lite rtab_explore.launch
