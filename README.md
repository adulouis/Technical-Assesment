# TurtleBot3
<img src="https://raw.githubusercontent.com/ROBOTIS-GIT/emanual/master/assets/images/platform/turtlebot3/logo_turtlebot3.png" width="300">

- Active Branches: noetic, humble, jazzy, main
- Legacy Branches: *-devel

<<<<<<< HEAD
## Open Source Projects Related to TurtleBot3
- [turtlebot3](https://github.com/ROBOTIS-GIT/turtlebot3)
- [turtlebot3_msgs](https://github.com/ROBOTIS-GIT/turtlebot3_msgs)
- [turtlebot3_simulations](https://github.com/ROBOTIS-GIT/turtlebot3_simulations)
- [turtlebot3_manipulation](https://github.com/ROBOTIS-GIT/turtlebot3_manipulation)
- [turtlebot3_manipulation_simulations](https://github.com/ROBOTIS-GIT/turtlebot3_manipulation_simulations)
- [turtlebot3_applications](https://github.com/ROBOTIS-GIT/turtlebot3_applications)
- [turtlebot3_applications_msgs](https://github.com/ROBOTIS-GIT/turtlebot3_applications_msgs)
- [turtlebot3_machine_learning](https://github.com/ROBOTIS-GIT/turtlebot3_machine_learning)
- [turtlebot3_autorace](https://github.com/ROBOTIS-GIT/turtlebot3_autorace)
- [turtlebot3_home_service_challenge](https://github.com/ROBOTIS-GIT/turtlebot3_home_service_challenge)
- [hls_lfcd_lds_driver](https://github.com/ROBOTIS-GIT/hls_lfcd_lds_driver)
- [ld08_driver](https://github.com/ROBOTIS-GIT/ld08_driver)
- [open_manipulator](https://github.com/ROBOTIS-GIT/open_manipulator)
- [dynamixel_sdk](https://github.com/ROBOTIS-GIT/DynamixelSDK)
- [OpenCR-Hardware](https://github.com/ROBOTIS-GIT/OpenCR-Hardware)
- [OpenCR](https://github.com/ROBOTIS-GIT/OpenCR)
=======
## Install Dependencies
### Install Cartographer
- sudo apt install ros-humble-cartographer
- sudo apt install ros-humble-cartographer-ros
### Install Navigation Stack for ROS2
- sudo apt install ros-humble-navigation2
-  sudo apt install ros-humble-nav2-bringup
>>>>>>> refs/remotes/origin/master

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
