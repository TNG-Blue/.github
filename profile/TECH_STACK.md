# Tech Stack

| Domain | Tools |
|--------|-------|
| **Robotics** | ROS 2 Humble (Foxy legacy), Nav2, RViz2, colcon, Gazebo Harmonic |
| **Perception / AI** | Isaac ROS, NanoOWL, TensorRT (FP16/INT8), PyTorch, ONNX, OpenCV, NVIDIA VPI |
| **GPU** | CUDA (`sm_87`), JetPack 6.2+, Nsight Systems, `tegrastats` |
| **Control & estimation** | PID with filtered D + anti-windup, LQR/LQG, MPC, FOC, Kalman/EKF, complementary filters |
| **Modelling** | MATLAB, Simulink, Embedded Coder, System Identification |
| **Embedded** | STM32N6 / STM32H7, ESP32, OpenMV · STM32CubeMX/IDE · FreeRTOS, Mbed OS · TrustZone |
| **Buses** | UART, SPI, I²C, CAN, Ethernet (UDP), USB, micro-ROS, MAVLink |
| **Languages** | Python, C++17, C99, CUDA C++, Go, MATLAB, Bash |
| **DevOps** | Docker, Kubernetes, Helm, GitHub Actions, MkDocs Material |
| **Hardware** | Jetson Orin Nano Super, Jetson Nano, Portenta H7, LiDAR, IMU, GNSS, encoders, BLDC/ESC |

## Engineering rules we hold ourselves to

1. Every control path is derived, not tuned by feel: plant model, filter, estimator, controller,
   saturation, failsafe — closed loop by default.
2. Stability evidence ships with the change: gain margin ≥ 6 dB, phase margin ≥ 45°
   (delays included), or a Lyapunov argument for nonlinear designs.
3. Verification order: model → SIL → HIL → bench → vehicle.
4. Apache-2.0 headers, Conventional Commits, SemVer changelogs.
