# Arduino-Robot-Arm-installation.
**installing  of the Arduino robot arm.**

**1-Creating ros workspace :** 
--------------------------
**--Input these commands terminal:**


 **source /opt/ros/noetic/setup.bash**
 
 **mkdir -p ~/catkin_ws/src**
 
 **cd ~/catkin_ws/** 
 
 **catkin_make**
 
 **source devel/setup.bash**
 
2-Installing Arduino Robot Arm Package
 -------------------------------------
 **--add the ardunino robot arm package to the src folder.
 by type these commands :**
 
 
 cd catkin_ws/src/
 
 sudo apt install git
 
 git clone https://github.com/smart-methods/arduino_robot_arm
 

**--install all the necessary dependencies**

 cd catkin_ws

 sudo apt-get install ros-noetic-moveit
 
 sudo apt-get install ros-noetic-joint-state-publisher ros-noetic-joint-state-publisher-gui
 
 sudo apt-get install ros-noetic-gazebo-ros-control joint-state-publisher
 
 sudo apt-get install ros-noetic-ros-controllers ros-noetic-ros-control

 
 **--compile all packages in your src folder**
 
 catkin_make
 
 Check your installation:
 -------------------------
 **--Before running anything on ROS you need to set your source setup file.**

source /home/"USER-NAME"/catkin_ws/devel/setup.bash

**"USER_NAME" Change it to your local username**


**Open the robot arm in Gazebow method:**

roslaunch robot_arm_pkg check_motors_gazebo.launch


![image](https://user-images.githubusercontent.com/109751319/186707920-fb3b0725-424a-4c1b-8a0f-de8435a81273.jpeg)
