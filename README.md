# Multi-Agent-Robotics (MAR)
In this repository, We are using 
1. [Linux (ubuntu-18.04)](https://www.youtube.com/watch?v=DC89AryJEE8&t=329s)
2. [ROS (Robot Operating System)](http://wiki.ros.org/melodic/Installation/Ubuntu)
3. [Gazebo (ROS Simulating Software)](http://gazebosim.org/tutorials?tut=install_ubuntu)
4. Python-IDE (like [Anaconda]()) and [Python](https://www.youtube.com/watch?v=z3Hdewxuuoo)(Ver-2 and Ver-3 both) in Command Prompt/linux.
5. You need to create your own catkin workspace
for that follow this link http://wiki.ros.org/catkin/Tutorials/create_a_workspace
after creating catkin workspace you need to create a package inside that workspace to do so follow this link
http://wiki.ros.org/ROS/Tutorials/CreatingPackage
remember for creating a package you must follow this command<br/>
```sh
$ catkin_create_pkg m2wr_description std_msgs urdf rospy roscpp
```
after that, you need to copy the contents from my [m2wr_description](https://github.com/shyammarjit/Multi-Agent-Robotics-MAR/tree/main/catkin_ws/src/m2wr_description)  and paste those inside your m2wr_description folder.<br/>You need to check your catkin workspace content and whatever content are not present in your workspace just copy from my catkin workspace and paste it in the proper directory.
For git cloning this repository use the following command
<br/>
```sh
$ git clone https://github.com/shyammarjit/Multi-Agent-Robotics-MAR
```

6.
