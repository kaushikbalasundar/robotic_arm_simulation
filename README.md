# robotic_arm_simulation
A test simulation of a robotic arm to explore basic features of ROS

This repository contains the simulation of a robotic arm. This was done in order to gain experience with some nice features of ROS: robot description using urdf and xacro, simulation in Gazebo, joint-space control of the arm,and finally inverse kinematics and motion planning with MoveIt!.

### **Usage**

**Install dependencies:**

rosdep install --from-paths src --ignore-src -r -y

Follow the instructions to set up a workspace and a package as in the PDF documentation. 

cd ~/catkin_ws/src/

**Clone this repository inside src:**

git clone https://github.com/kaushikbalasundar/robotic_arm_simulation

**Build catkin workspace in the catkin_ws directory:**

cd ..

catkin_make

**Init the environment:**

source devel/setup.sh

**Launch the gazebo simulation with position controllers in the launch folder:**

roslaunch position_controllers.launch

**Launch rqt_gui**

rosrun rqt_gui rqt_gui

**Launch the MoveIt! move group to control the end effector:**

roslaunch moveit_ardop2_1 demo.launch

You can now use the MoveIt! plugin in Rviz to control the arm. 

**Images:**

![gazebo_joint_controller](https://user-images.githubusercontent.com/44526371/47739612-be90c380-dc9b-11e8-8d33-499090547f85.png)


![moveit_](https://user-images.githubusercontent.com/44526371/47739618-c3557780-dc9b-11e8-999a-fca53b56f143.png)

**Videos**

![gazebo_joint_controller](https://user-images.githubusercontent.com/44526371/47739582-af117a80-dc9b-11e8-9cb8-64dd14c14351.gif)

![moveit](https://user-images.githubusercontent.com/44526371/47739593-b6388880-dc9b-11e8-8f9a-56ecc2e2b8f4.gif)


