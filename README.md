# Multi-Agent-Robotics (MAR)
In this repository, We are using 
1. Linux (ubuntu-18.04)
2. ROS (Robot Operating System)
3. Gazebo (ROS Simulating Software)
4. Python-IDE (like Anaconda) and Python(ver-2 and ver-3 both) in Command Prompt.
Step-1
You need to install Ubuntu-18.04
for that, you can follow this link to use that
https://www.youtube.com/watch?v=DC89AryJEE8&t=329s
Step-2
You need to install ROS-Melodic
http://wiki.ros.org/melodic/Installation/Ubuntu
then you need to create your own catkin workspace
for that follow this link
http://wiki.ros.org/catkin/Tutorials/create_a_workspace
after creating catkin workspace you need to create a package inside that workspace
http://wiki.ros.org/ROS/Tutorials/CreatingPackage
remember for creating a package you must follow this command
$ catkin_create_pkg m2wr_description std_msgs urdf rospy roscpp
after that, you need to copy the contents from my URDF folder []  and paste those inside your urdf folder.
