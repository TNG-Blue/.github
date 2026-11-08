# Research

## Focus

| Area | Questions we work on |
|------|----------------------|
| **Edge perception** | Real-time open-vocabulary detection under Jetson power and memory limits |
| **State estimation** | Consistent multi-sensor fusion (IMU, GNSS, LiDAR, encoders); NIS/NEES-validated filters |
| **Flight control** | Model-based control of a coaxial X12 hexacopter: cascaded attitude/rate loops, MPC, FOC drives |
| **GNSS-denied navigation** | LiDAR/visual SLAM and odometry when satellite fixes drop out |
| **Embedded safety** | TrustZone partitioning, watchdogs and defined failsafe states on STM32N6 |

## Roadmap

- **Now:** HIL test rig for the flight controller; TensorRT INT8 for NanoOWL
- **Next:** pose-graph SLAM back-end; MPC with constraint handling on the Jetson
- **Later:** multi-robot coordination between UAV and ground robot

## References we build on

Åström & Murray — *Feedback Systems* · Franklin, Powell & Workman — *Digital Control of Dynamic
Systems* · Simon — *Optimal State Estimation* · Rawlings, Mayne & Diehl — *Model Predictive
Control* · Thrun, Burgard & Fox — *Probabilistic Robotics* · Groves — *Principles of GNSS,
Inertial, and Multisensor Integrated Navigation Systems*

## Collaborate

Open to collaboration on edge AI, estimation and UAV control — open an
[issue](https://github.com/TNG-Blue/Isaac_ROS-Jetbot_NanoOWL-Docs/issues) or email
nguyen_danh_2002@outlook.com.
