# Drone_URDF
ROS 2 Jazzy Harmonic package containing the URDF and Xacro descriptions for a quadrotor drone. 
It includes 3D meshes, modular Xacro files, and launch configurations for RViz and Gazebo simulation.
Gazebo-ready with simulation launch files  RViz launch file for visualization
Modular URDF/Xacro structure

Installation

1. Clone the repository into your ROS 2 workspace:
cd ~/ros2_ws/src
git clone https://github.com/kowsik16/droneis_description.git

2.Install dependencies:
sudo apt update && rosdep update
rosdep install --from-paths src --ignore-src -r -y

3.Build the package:
cd ~/ros2_ws
colcon build --packages-select droneis_description
source install/setup.bash

To visualize the drone model in RViz:
ros2 launch droneis_description display.launch.py

To launch the drone in Gazebo:
ros2 launch droneis_description gazebo.launch.py
