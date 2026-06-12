# Energy-Aware Robotic 3D Printing Simulation with UR5e (ROS + MoveIt + Gazebo)
<img width="800" height="552" alt="Demo_Printing-ezgif com-video-to-gif-converter" src="https://github.com/user-attachments/assets/88d2f8cc-1753-4f05-95d7-60fed65dab7d" />



## 📌 Overview

This project presents a simulation framework for energy-aware robotic 3D printing using the UR5e manipulator in a Gazebo environment. The system integrates motion planning, trajectory execution, and energy consumption estimation to evaluate the efficiency of different toolpath strategies.

The goal is to optimize printing trajectories not only for geometric accuracy but also for **energy efficiency**, which is critical for sustainable and large-scale robotic additive manufacturing.

---

## 🚀 Key Features

* 🤖 **UR5e Simulation in Gazebo**

  * Full robot simulation with ROS integration
  * Realistic kinematics and dynamics

* 🧭 **Motion Planning with MoveIt**

  * Collision-aware trajectory planning
  * Smooth path generation for printing tasks

* 🔋 **Energy Consumption Modeling**

  * Estimates energy usage during trajectory execution
  * Enables comparison of different toolpaths

* 🧩 **Custom Path Planning for 3D Printing**

  * Supports structured printing paths (e.g., layers, contours)
  * Flexible trajectory generation

---

## 🏗️ System Architecture

```id="5s7e0l"
User-defined Toolpath
          ↓
   Path Planning Module
          ↓
    MoveIt Motion Planning
          ↓
 Trajectory Execution (ROS)
          ↓
      Gazebo Simulation
          ↓
 Energy Consumption Estimation
```

---

## ⚙️ Methodology

### 1. Path Planning

Custom toolpaths are generated for 3D printing tasks, including layer-based or contour-based trajectories.

### 2. Motion Planning (MoveIt)

The planned path is converted into joint-space trajectories using MoveIt, ensuring smooth and collision-free motion.

### 3. Simulation Execution

The trajectory is executed in the Gazebo environment with the UR5e robot model.

### 4. Energy Estimation

Energy consumption is estimated based on:

* Joint velocities
* Motion duration
* Control effort (torque approximation)

---

## 🧪 Experimental Setup

* Robot: UR5e (Universal Robots)
* Framework: ROS + MoveIt
* Simulator: Gazebo
* Planning: MoveIt Motion Planning Pipeline
* Control: Joint trajectory execution

---

## 📊 Results

* Demonstrated smooth and feasible printing trajectories
* Compared energy consumption across different path strategies
* Showed trade-offs between path length, smoothness, and energy usage

---

## 🔬 Research Contributions

This project contributes:

* A simulation pipeline for **energy-aware robotic additive manufacturing**
* Integration of **motion planning and energy modeling**
* A framework for evaluating trajectory efficiency in robotic printing

---

## 🎥 Demo

(Add simulation video or GIF here)

---

## 📜 License

MIT License
