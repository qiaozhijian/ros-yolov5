# YOLOv5-ROS
### Introduction
This is a package combined with ROS melodic and YOLOv5. In this package, C++ and python are working together. You don't have to prepare dataset and model. Just do it!
### Environment and Dependencies
Code was tested using Python 3.8 with PyTorch 1.7.1 and MinkowskiEngine 0.5.0 on Ubuntu 18.04 with CUDA 10.2.
The following Python packages are required:
* PyTorch (version >= 1.7)
* catkin-simple
* rospkg
* ros-melodic-ros-numpy
### Directory
Your_workspace  
├── build  
├── devel  
└── src  
   ├── catkin_simple  
   ├── CMakeLists.txt  
   └── ros-yolov5  
### Run
````
cd Your_workspace/src
git clone https://github.com/qiaozhijian/ros-yolov5.git
git clone https://github.com/catkin/catkin_simple.git
cd .. && catkin_make
pip install rospkg
sudo apt install ros-melodic-ros-numpy
source devel/setup.bash
roslaunch ros_yolo service_demo.launch
````