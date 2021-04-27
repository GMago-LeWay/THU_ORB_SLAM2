# Build 与 run 方法
## build
参考链接：https://zhuanlan.zhihu.com/p/29629824

## run
参考展示PPT
- 数据集(TUM/..)
运行SLAM命令例：
./Examples/Monocular/mono_tum Vocabulary/ORBvoc.txt Examples/Monocular/TUMX.yaml PATH_TO_SEQUENCE_FOLDER
主程序 词典位置 配置文件位置 对应数据集位置 
- USB相机(需提前安装usb_cam的ROS包)
先启动相机节点
roslaunch usb_cam usb_cam-test.launch
运行SLAM命令例：
rosrun ORB_SLAM2 Mono /home/liwei/Desktop/SLAM/catkin_ws/src/ORB/Vocabulary/ORBvoc.txt /home/liwei/Desktop/SLAM/catkin_ws/src/ORB/Examples/ROS/ORB_SLAM2/Asus.yaml
rosrun ORB_SLAM2 模式 词典位置 配置文件位置
 