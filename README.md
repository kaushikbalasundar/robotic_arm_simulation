# robotic_arm_simulation
A test simulation of a robotic arm to explore basic features of ROS

This repository contains the simulation of a robotic arm. This was done in order to gain experience with some nice features of ROS: robot description using urdf and xacro, simulation in Gazebo, joint-space control of the arm,and finally inverse kinematics and motion planning with MoveIt!.

###**Usage**

**Install dependencies:**

rosdep install --from-paths src --ignore-src -r -y

**Build catkin workspace:**

catkin_make

**Init the environment:**

source devel/setup.sh

**Launch the gazebo simulation with position controllers in the launch folder:**

roslaunch position_controllers.launch

**Launch rqt_gui**

rosrun rqt_gui rqt_gui

**Launch the MoveIt! move group to control the end effector:**

roslaunch demo.launch 

You can now use the MoveIt! plugin in Rviz to control the arm.
