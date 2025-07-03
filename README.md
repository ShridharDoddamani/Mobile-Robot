# Mobile-Robot

**Objective**: Simulate an autonomous mobile robot equipped with a manipulator arm to perform pick-and-place tasks in a structured environment using ROS. This project demonstrates multi-domain integration: navigation, perception, and manipulation.

---

## Tools & Frameworks

- **ROS**: ROS2 Humble / ROS Noetic  
- **Simulator**: Gazebo / CoppeliaSim  
- **Navigation**: ROS Navigation Stack / SLAM Toolbox  
- **Motion Planning**: MoveIt for the manipulator  
- **Sensors**: Simulated RGB-D Camera / Lidar  

---

## Key Features

-  Autonomous navigation to pick & place zones  
-  Object detection using simulated RGB-D or predefined coordinates  
-  Pick-and-place with 4-6 DOF robotic arm  
-  Integration of mobile base and manipulator in a single robot model  
-  Environment includes table, walls, dynamic/static obstacles  

---

## System Overview

1. **Localization & Mapping**:
   - Uses 2D SLAM or AMCL to localize robot in the environment.
2. **Path Planning**:
   - Uses Dijkstra/A* or NavFn to reach the pick zone.
3. **Object Detection**:
   - Uses fixed positions or simulated vision (OpenCV or YOLO if extended).
4. **Pick and Place**:
   - The robotic arm performs pick and place using MoveIt and trajectory execution.
5. **Loop**:
   - After placing, returns to start or moves to another object.
