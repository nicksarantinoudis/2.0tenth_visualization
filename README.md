# 2.0tenth_visualizatioin
A visualization package for the 2.0 Tenth platform in order to visualize
real-time data or pre-recorded ROS bags. 

## ROS2 Build
1. Create your workspace folder
2. Create a src folder
3. Run `colcon build` on the empty folder to initialize
5. Clone the repository into the src folder
6. Run `rosdep update`
7. Run `rodep install --from-paths src -i -y`
8. Run `colcon build`

The build should be succesfully completed

## Tips 

Don't forget to `source /opt/ros/humble/setup.bash` if not 
in your `.bashrc` file.
Also `source install/setup.bash` on your workspace after the 
succesful build 

## Launch Files
There is 1 useful `.launch` file which can be used for testing

1. `ros2 launch f1_tenth_visualization f1_tenth_visualization.launch.py` -> Visualizes 
real time or pre-recorded data files (in ROS bag format) through RViz. Data can be also
streamed to a different machine over Wi-Fi as long as both have the same `ROS_DOMAIN_ID`
