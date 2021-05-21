# Multi-Agent-Robotics (MAR)
# Part-1: Installing the Robots
For git cloning this repository use the following command
<br/>
```sh
$ git clone https://github.com/shyammarjit/Multi-Agent-Robotics-MAR
```

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
after that, you need to copy the contents from my [worlds](https://github.com/shyammarjit/Multi-Agent-Robotics-MAR/tree/main/catkin_ws/src/worlds) folder to your folder.
You need to copy the contents from my [launch](https://github.com/shyammarjit/Multi-Agent-Robotics-MAR/tree/main/catkin_ws/src/m2wr_description/launch) folder to your launch folder and also you need to copy the contents from my [urdf](https://github.com/shyammarjit/Multi-Agent-Robotics-MAR/tree/main/catkin_ws/src/m2wr_description/urdf) folder to your urdf folder.<br/>You need to check your catkin workspace content and whatever content are not present in your workspace just copy from my catkin workspace and paste it in the proper directory.<br/>
6. heck your [launch files](https://github.com/shyammarjit/Multi-Agent-Robotics-MAR/tree/main/catkin_ws/src/m2wr_description/launch)<br/>

7. Launch RViz:
```sh
$ roslaunch m2wr_description rviz.launch 
```

8. Launch Gazebo:
```sh
$ roslaunch gazebo_ros empty_world.launch
```

9. Load our Model:
```sh
$ roslaunch m2wr_description spawn_m.launch 
```
# Part-2 Controlling the Robot using KeyBoard
To Install Teleop-Twist-Keyboard use 
```sh
$ sudo apt-get install ros-melodic-teleop-twist-keyboard
$ cd ~/catkin_ws/src
$ git clone https://github.com/ros-teleop/teleop_twist_keyboard
$ cd ~/catkin_ws
$ catkin_make
$ source ~/catkin_ws/devel/setup.bash
$ source ~/.bashrc
```
I also assume that you have your ros environment in your bashrc file. It should contain the following lines : 
```sh
source /opt/ros/melodic/setup.bash
```
and you should add the following lines to your bashrc script by running :
```sh
$ gedit ~/.bashrc and add :
$ source ~/catkin_ws/devel/setup.bash
```
open terminal and run

Run the following code in order to control the robot using the keyboard:
```sh
$ rosrun teleop_twist_keyboard teleop_twist_keyboard.py
```
