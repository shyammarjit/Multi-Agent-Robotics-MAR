# Multi-Agent-Robotics (MAR)
In this repository, We are using 
1. [Linux (ubuntu-18.04)](https://www.youtube.com/watch?v=DC89AryJEE8&t=329s)
2. [ROS (Robot Operating System)](http://wiki.ros.org/melodic/Installation/Ubuntu)
3. [Gazebo (ROS Simulating Software)](http://gazebosim.org/tutorials?tut=install_ubuntu)
4. Python-IDE (like [Anaconda]()) and [Python](https://www.youtube.com/watch?v=z3Hdewxuuoo)(Ver-2 and Ver-3 both) in Command Prompt/linux.
5. You need to create your own [catkin workspace](http://wiki.ros.org/catkin/workspaces)
for that use the following commands
```sh
$ mkdir -p ~/catkin_ws/src
$ cd ~/catkin_ws/
$ catkin_make
```
after creating catkin workspace you need to create a [package](http://wiki.ros.org/ROS/Tutorials/CreatingPackage) inside that workspace to do so follow the following commands
```sh
$ cd ~/catkin_ws/src/
$ catkin_create_pkg m2wr_description std_msgs urdf rospy roscpp
$ mkdir worlds
$ cd ~/catkin_ws/src/m2wr_description/
$ mkdir launch
$ mkdir urdf
```
after that, you need to copy the contents from my [m2wr_description](https://github.com/shyammarjit/Multi-Agent-Robotics-MAR/tree/main/catkin_ws/src/m2wr_description) and paste those inside your m2wr_description folder.<br/>You need to check your catkin workspace content and whatever content are not present in your workspace just copy from my catkin workspace and paste it in the proper directory.
For git cloning this repository use the following command
<br/>
```sh
$ git clone https://github.com/shyammarjit/Multi-Agent-Robotics-MAR
```

6. check your [launch files](https://github.com/shyammarjit/Multi-Agent-Robotics-MAR/tree/main/catkin_ws/src/m2wr_description/launch)
7. Launch rviz:
```sh
$ roslaunch m2wr_description rviz.launch 
```

8. Launch gazebo:
```sh
$ roslaunch gazebo_ros empty_world.launch
```

9. Load our model:
```sh
$ roslaunch m2wr_description spawn.launch 
```

10. Run the following code in order to control the robot using the keyboard:
```sh
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
