## 环境
**操作系统**：Ubuntu 22.04  
**ROS 2**：Humble  
**Gazebo**：classic
## 依赖
```
sudo apt install ros-humble-robot-state-publisher
sudo apt install ros-humble-joint-state-publisher
sudo apt install ros-humble-xacro
sudo apt install ros-humble-gazebo-ros-pkgs
sudo apt install ros-humble-ros2-control
sudo apt install ros-humble-ros2-controllers
sudo apt install ros-humble-gazebo-ros2-control
```
可能有多余的依赖，但不知道是哪些，全装上就是了。
##  构建包
```
mkdir bbr_car_ws/src && cd bbr_car_ws/src
git clone https://github.com/DDTRobot/TITA_Description.git
```
