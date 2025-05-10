## 环境
**操作系统**：Ubuntu 22.04  
**ROS 2**：Humble  
**Gazebo**：classic
## 依赖
```
sudo apt install ros-$ROS_DISTRO-robot-state-publisher
sudo apt install ros-$ROS_DISTRO-joint-state-publisher
sudo apt install ros-$ROS_DISTRO-xacro
sudo apt install ros-$ROS_DISTRO-gazebo-ros-pkgs
sudo apt install ros-$ROS_DISTRO-gazebo-ros2-control
sudo apt install ros-$ROS_DISTRO-ros2-control
sudo apt install ros-$ROS_DISTRO-ros2-controllers
```
可能有多余的依赖，但不知道是哪些，全装上就是了。
##  构建包
```
mkdir -p bbr_car_ws/src && cd bbr_car_ws/src
git clone https://github.com/chenanjie233/bbr_car_description.git
cd ..
colcon build
source install/setup.bash
ros2 launch bbr_robot_description gazebo_sim.launch.py
```
可用ros2自带的键盘控制节点控制小车轮子，重新打开一个终端，输入以下命令
```
ros2 run teleop_twist_keyboard teleop_twist_keyboard 
```
