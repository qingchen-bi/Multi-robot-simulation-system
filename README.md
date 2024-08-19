**This multi-robot simulation system is suitable for Gazebo, which has been tested under Ubuntu 18.04.**
This system can be used to support multi-robot exploration, navigation, SLAM, and other tasks.

This system uses Scout 2.0 robots, where the visualization rendering of the robot body is disabled. 
Sensors can be selected from VLP-16 and HDL-32. 
Please install the Scout robot dependency and Velodyne sensor dependency yourself. 
The code for obtaining the ground truth of robots in Gazebo refers to some of the code in **FAEL**.

$ roslaunch simworld three_scout.launch

### For Ubuntu 20.04,

You need to modify the relevant content of CmakeLists.txt in sensor_conversion to "add compile_options (- std=c++14)"
