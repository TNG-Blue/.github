<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:0A1F44,100:00D4FF&height=180&section=header&text=TNG-Blue&fontSize=60&fontColor=ffffff&fontAlignY=35&desc=Autonomous%20robotics%20at%20the%20edge&descSize=18&descAlignY=58" width="100%" alt="TNG-Blue" />

<img src="https://readme-typing-svg.demolab.com?font=JetBrains+Mono&weight=600&size=18&duration=2800&pause=800&color=00D4FF&center=true&vCenter=true&width=620&lines=GPU+perception+on+NVIDIA+Jetson;Model-based%2C+closed-loop+control;Embedded+firmware+on+STM32N6;From+Simulink+to+SIL%2C+HIL+and+flight" alt="Typing headline" />

[![Docs](https://img.shields.io/badge/Docs-Isaac__ROS--Jetbot__NanoOWL-00D4FF?style=for-the-badge&logo=materialformkdocs&logoColor=white)](https://tng-blue.github.io/Isaac_ROS-Jetbot_NanoOWL-Docs/)
![License](https://img.shields.io/badge/License-Apache--2.0-0A1F44?style=for-the-badge)

</div>

## 🚁 Flagship — Isaac_ROS-Jetbot_NanoOWL

A Jetson Orin Nano Super platform for a **coaxial X12 hexacopter** and a **ground robot**:
open-vocabulary perception with NanoOWL, sensor fusion, flight control, simulation and OTA updates.

```mermaid
flowchart LR
  S[Sensors<br/>IMU · GNSS · LiDAR · camera] --> F[Filter] --> E[Estimator<br/>KF / EKF] --> C[Controller<br/>PID · LQR · MPC · FOC] --> A[Actuators<br/>12 × BLDC] --> P((Plant))
  P -. feedback .-> S
```

<table>
  <tr>
    <td width="33%" valign="top">
      <b>👁️ Perception</b><br/>
      Isaac ROS · NanoOWL<br/>TensorRT · CUDA <code>sm_87</code> · VPI
    </td>
    <td width="33%" valign="top">
      <b>🎛️ Control</b><br/>
      Derived, closed-loop designs<br/>GM ≥ 6 dB · PM ≥ 45°
    </td>
    <td width="33%" valign="top">
      <b>🔧 Embedded</b><br/>
      STM32N6 · FreeRTOS · TrustZone<br/>Portenta H7 · ESP32 · OpenMV
    </td>
  </tr>
</table>

## 🛠️ Stack

<div align="center">

<img src="https://skillicons.dev/icons?i=ros,py,cpp,c,go,matlab,opencv,pytorch,docker,kubernetes,ubuntu,cmake,arduino,githubactions&perline=14" alt="Tech stack" />

![NVIDIA Jetson](https://img.shields.io/badge/NVIDIA-Jetson-76B900?style=flat-square&logo=nvidia&logoColor=white)
![CUDA](https://img.shields.io/badge/CUDA-TensorRT-76B900?style=flat-square&logo=nvidia&logoColor=white)
![ROS 2](https://img.shields.io/badge/ROS%202-Humble-22314E?style=flat-square&logo=ros&logoColor=white)
![Gazebo](https://img.shields.io/badge/Gazebo-Harmonic-F58113?style=flat-square)
![STM32](https://img.shields.io/badge/STM32-N6-03234B?style=flat-square&logo=stmicroelectronics&logoColor=white)

</div>

## 📌 More

[Projects](https://github.com/TNG-Blue/.github/blob/master/profile/PROJECTS.md) ·
[Tech stack](https://github.com/TNG-Blue/.github/blob/master/profile/TECH_STACK.md) ·
[Research](https://github.com/TNG-Blue/.github/blob/master/profile/RESEARCH.md) ·
[Documentation](https://tng-blue.github.io/Isaac_ROS-Jetbot_NanoOWL-Docs/)

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:00D4FF,100:0A1F44&height=100&section=footer" width="100%" alt="" />
