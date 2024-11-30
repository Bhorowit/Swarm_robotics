# Swarm Robotics Project

## Overview
This project demonstrates a swarm robotics system using ROS 2, Python, and the A* algorithm. It features:
- A* pathfinding for autonomous navigation.
- Master-slave synchronization for task assignment.
- Dynamic obstacle handling for real-time path replanning.

## System Architecture
- *talker.py*: The master node that assigns tasks.
- *listener.py*: The slave node that calculates paths and handles obstacles.

## Installation
1. Clone the repository:
   ```bash
   cd ~/ros2_ws/src
   git clone <your-repository-url>
   ```

2.	Build the workspace:
  ```bash
  cd ~/ros2_ws
  colcon build
  source install/setup.bash
  ```

## Usage
1.	Start the master node:
   ```bash
   ros2 run swarm_robots talker
   ```
2. Start the slave node:
   ```bash
   ros2 run swarm_robots listener
   ```

## Future Work

•	Integration with Gazebo for 3D visualization.
•	Multi-robot coordination for swarm behaviors.
