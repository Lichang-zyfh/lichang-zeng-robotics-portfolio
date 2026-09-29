# Lichang Zeng | Robotics Portfolio

Robotics Engineering undergraduate at **Xi'an Jiaotong-Liverpool University (XJTLU)**, building learning-enabled robotic systems that connect perception, decision-making, and physical action.

My current focus is **learning-based whole-body control and simulation-to-real transfer for contact-rich humanoid robots**. Across research, internships, and hardware projects, I have worked from embedded firmware and robot perception to reinforcement learning, ROS2 navigation, and real-world manipulation.

> **Current direction:** embodied intelligence algorithms and robust motion control for deployable robots.

## Featured work

### Humanoid Whole-Body Balance and Target-Reaching Control *(Final Year Project — in progress)*

**[Project repository](https://github.com/Lichang-zyfh/FYP)**  
**Platform:** Unitree H1-2 humanoid robot · Isaac Lab · PPO

I am developing a simulation-first study of whole-body standing balance during single-arm 3D target reaching. The central question is whether a unified policy can coordinate reaching and balance, and whether structured advantage assignment and balance-aware rewards improve this coordination.

- Compare an IK/PD standing baseline with Vanilla PPO, Advantage Mixing PPO, and CoM- and ZMP-reward variants.
- Use a 21-DoF joint-position policy while the low-level PD controller tracks actions at 50 Hz.
- Evaluate target-reaching success, balance/fall safety, disturbance recovery, action smoothness, and control effort under target, payload, push, and dynamics variation.
- Follow a reproducible protocol with fixed training/evaluation conditions, five training seeds, held-out evaluation scenarios, checkpoints, and experiment manifests.

**Status:** experiment specification and simulator/asset-validation stages completed; formal training and evaluation are forthcoming. No sim-to-real or performance claim is made before these experiments are complete.

---

### Friendy: Embodied Multimodal AI Desktop Tutor

**[Source code](https://github.com/Lichang-zyfh/ENT208TC-Friendy)** · **[Demo video](https://www.youtube.com/watch?v=vNoVkv8muMY)**  
**Stack:** M5Stack CoreS3 / ESP32 · C++ · Python · OpenCV · EasyOCR · VLM · Vosk

Friendy is an embodied AI tutor that converts a spoken hardware question into physical guidance. A camera observes the workspace; local OCR and a cloud vision-language model identify the requested component; a two-axis laser gimbal then points to it.

- Built an edge–hub–cloud system: embedded actuation on CoreS3, perception/orchestration on a Python hub, and semantic reasoning through a VLM.
- Implemented global-anchor homography calibration to map image locations to pan/tilt laser commands, with software limits to protect the hardware.
- Integrated offline speech recognition, OCR, JSON-based tool commands, I2C/PWM control, Wi-Fi video streaming, and serial communication.
- Iterated through hardware and cross-layer failures, including servo current issues, I2C deadlock, timing, and threading problems.

---

### 12-DoF Bipedal Robot: Vision-Based Autonomous Navigation and Target Touching

**[Demo video](https://www.youtube.com/watch?v=eSwz9dzyCuo)**  
**Stack:** ESP32 · PlatformIO · ESP32-CAM · YOLOv8 · Wi-Fi control

Developed a 12-DoF bipedal robot that detects obstacles and targets, estimates their relative position from monocular vision, and executes navigation and target-touching behaviors.

- Developed ESP32 firmware and a browser-based servo calibration/debugging tool.
- Collected and annotated a custom image dataset; trained and deployed a YOLOv8 object detector.
- Designed an upper-computer vision / lower-controller motion architecture with real-time Wi-Fi commands.
- Learned first-hand how actuator limits, calibration, and compute constraints shape practical robot control.

---

### Autonomous Navigation and SLAM on TurtleBot3

**[Demo video](https://www.youtube.com/watch?v=VpFFS7rriPE)**  
**Stack:** ROS2 · Gazebo · TurtleBot3 Waffle · Cartographer · Nav2 · AMCL

Designed, simulated, and deployed an indoor mobile-robot navigation workflow from mapping to autonomous execution.

- Built a ROS2–Gazebo digital twin and used Cartographer for LiDAR mapping.
- Deployed AMCL localization and the Nav2 navigation stack on TurtleBot3 Waffle.
- Implemented a Python middleware node that corrected message-type and timestamp incompatibilities between the navigation stack and low-level hardware interface.

---

### Vision-Based Autonomous Line-Tracking Robot

**[Demo video](https://www.youtube.com/watch?v=0a2DnCCf1dk)**  
**Stack:** Raspberry Pi 5 · OpenCV · PID control · IMU · MATLAB · SolidWorks

Built an autonomous line-following mobile robot for environmental monitoring.

- Designed the chassis and test track in SolidWorks.
- Used OpenCV to detect a blue guidance line and PID control to regulate steering and speed.
- Logged temperature/humidity, voltage/current, and trajectory data; used MATLAB for analysis and visualization.

---

### Autonomous Vision-Based Grasping and Manipulation

**[Demo video](https://www.youtube.com/watch?v=uGvG3kty1Q8&t=28s)**  
**Platform:** 6-DoF Piper arm · Intel RealSense D405 · OpenCV

Developed a visual grasping pipeline for object pickup and placement in an unstructured workspace.

- Combined image segmentation, depth sensing, and forward kinematics to estimate grasp-relevant object positions.
- Executed autonomous grasp-and-place behavior with a 6-DoF robot arm.

## Research and engineering experience

- **Robot social navigation research:** Proposed an Interaction-Prior Attention Network for dynamic crowd navigation; evaluated against ORCA, SARL, and RGL using OOD environments, ablations, attention visualization, and trajectory analysis.
- **Chinese Academy of Sciences internship:** Developed FreeRTOS/ESP-IDF firmware for a tendon-driven dexterous hand; worked on adaptive grasping, load-sensing homing, tactile simulation, and PPO-based manipulation tasks.
- **Simulation and learning:** Experience with MuJoCo, Isaac Sim/Gym, Gazebo, PPO, tactile simulation, and robot-system debugging.

## Technical toolkit

`Python` · `C/C++` · `MATLAB` · `Linux` · `ROS2` · `MuJoCo` · `Isaac Sim / Isaac Lab` · `Gazebo` · `OpenCV` · `PyTorch / YOLOv8` · `ESP32 / ESP-IDF / FreeRTOS` · `PlatformIO`

## Links

- **YouTube demos:** [@曾李畅](https://www.youtube.com/@%E6%9B%BE%E6%9D%8E%E7%95%85)
- **GitHub:** [@Lichang-zyfh](https://github.com/Lichang-zyfh)
- **Email:** 15038572597@163.com

---

*I welcome conversations on humanoid whole-body control, reinforcement learning, robot perception, and real-world embodied AI systems.*
