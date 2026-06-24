# TurtleBot3
<img src="https://raw.githubusercontent.com/ROBOTIS-GIT/emanual/master/assets/images/platform/turtlebot3/logo_turtlebot3.png" width="300">

- Active Branches: humble, jazzy, main(rolling)
- Legacy Branches: *-devel, noetic

## Install Dependencies
### Install Cartographer
- sudo apt install ros-humble-cartographer
- sudo apt install ros-humble-cartographer-ros
### Install Navigation Stack for ROS2
- sudo apt install ros-humble-navigation2
-  sudo apt install ros-humble-nav2-bringup

## Starting the simulation
### Starting the Environment
- Source the environment: source ~/turtlebot3_ws/install/setup.bash
- Launch the environment: ros2 launch turtlebot3_gazebo empty_world.launch.py

## Starting the Goal Server
- Open a new terminal
- Source the environment: source ~/turtlebot3_ws/install/setup.bash
- Start the server: ros2 run turtlebot3_example turtlebot3_goal_service

## Calling the service
- ros2 service call turtlebot3_goal_server turtlebot3_msgs/srv/PoseCommand "{x: <x_position>, y: <y_position>, yaw: <yaw_angle>}"
