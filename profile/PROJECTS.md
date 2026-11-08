# Projects

> 🔒 Most source repositories are private; public material is linked where it exists.

| Project | Platform | Status |
|---------|----------|--------|
| [Isaac_ROS-Jetbot_NanoOWL](#isaac_ros-jetbot_nanoowl) | Jetson Orin Nano Super, STM32N6 | 🟢 Active |
| [JetOwl Flight Control / Vision](#jetowl-flight-control--vision) | STM32N657 | 🟢 Active |
| [Jetbot Nano](#jetbot-nano) | Jetson Nano, ESP32 | 🟡 Maintenance |
| [VPI Object Detection](#vpi-object-detection) | Jetson, NVIDIA VPI | 🟢 Stable |
| [Portenta H7](#portenta-h7) | STM32H747 (M7 + M4) | 🟡 Learning |

## Isaac_ROS-Jetbot_NanoOWL

Autonomous platform for a coaxial X12 hexacopter (12 BLDC + encoders) and a ground robot.

- **Perception:** Isaac ROS + NanoOWL open-vocabulary detection, TensorRT engines on `sm_87`
- **Estimation & control:** filtered sensors → KF/EKF → PID/LQR/MPC/FOC, closed loop, with
  derivations and stability margins documented per controller
- **Simulation:** Gazebo Harmonic plugin, MCU→Jetson Ethernet sensor link emulator, MATLAB/Simulink
- **Deployment:** Docker, Kubernetes/Helm, Go OTA server, MAVLink relay, Android companion app
- 📖 [Documentation site](https://tng-blue.github.io/Isaac_ROS-Jetbot_NanoOWL-Docs/)

## JetOwl Flight Control / Vision

STM32N657 firmware used as submodules of the platform above: flight and motor control (FOC,
FreeRTOS, TrustZone secure/non-secure split) and on-board vision.

## Jetbot Nano

ROS 2 mobile robot on Jetson Nano with an ESP32 motor/sensor bridge: object detection, obstacle
avoidance, camera-based navigation.

## VPI Object Detection

Hardware-accelerated classical vision on Jetson (NVIDIA VPI + OpenCV): colour segmentation,
contours, template and feature matching — no model training needed. Used for aquaculture counting.

## Portenta H7

Dual-core STM32H747 firmware (Cortex-M7 480 MHz + M4 240 MHz) with Mbed OS and STM32CubeMX:
RTOS scheduling, HAL drivers, inter-core communication.

## Next

| Item | Goal |
|------|------|
| Multi-robot coordination | Shared map and task allocation across UAV + ground robot |
| SLAM back-end | Loop closure and pose-graph optimisation |
| Sensor suite | LiDAR + depth fusion with consistency-checked estimators |
| Hardware-in-the-loop | Every controller verified MATLAB → SIL → HIL → bench → vehicle |
