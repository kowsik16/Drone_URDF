# Drone_URDF
ROS 2 Jazzy Harmonic package containing the URDF and Xacro descriptions for a quadrotor drone. 
It includes 3D meshes, modular Xacro files, and launch configurations for RViz and Gazebo simulation.
Gazebo-ready with simulation launch files  RViz launch file for visualization
Modular URDF/Xacro structure

### Installation

### Clone the Repository:

cd ~/your_workspace_name/src 

git clone https://github.com/kowsik16/Drone_URDF.git

### Install Dependencies:

sudo apt update && rosdep update

rosdep install --from-paths src --ignore-src -r -y


### Build the Package:

cd ~/your_workspace_name

colcon build --packages-select differential_drive_robot_with_lidar

source install/setup.bash


### Launch in RViz:

ros2 launch differential_drive_robot_with_lidar display.launch.py


### Launch in Gazebo:

ros2 launch differential_drive_robot_with_lidar gazebo.launch.py
