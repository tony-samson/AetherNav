# AetherNav
Stereo vision–based autonomous drone navigation using CNN and Visual SLAM

![Drone preview](imgs/preview.png)


# Stereo Vision–Based Autonomous Drone Navigation
## Project Description

This project focuses on developing a vision-based autonomous UAV navigation system using stereo cameras, deep learning, and Visual SLAM.

The system integrates a Raspberry Pi companion computer with a Pixhawk flight controller to enable real-time depth perception, obstacle detection, and waypoint-based navigation in GPS-denied environments.

The long-term objective is to transition from human-assisted decision approval to full autonomy using stereo vision and AI-based perception.

## Project Goals

 Implement uncalibrated stereo image rectification

 Generate disparity maps and estimate depth

 Train a CNN for obstacle classification and navigation decisions

 Integrate Stereo Visual SLAM for mapping and localization

 Enable human-in-the-loop assisted decision mode

 Deploy real-time waypoint navigation from Raspberry Pi

 Transition to fully autonomous flight

## System Architecture
### Hardware

Raspberry Pi 5 (Companion Computer)

HAILO AI HAT 26TOPS

Pixhawk Flight Controller

Dual Raspberry Pi Cameras (Stereo Setup)

MAVLink Communication Interface

### Software Stack

Python

OpenCV

PyTorch / TensorFlow

MAVSDK / DroneKit

Stereo Depth Estimation Algorithms

## Visual SLAM Pipeline

### Operational Pipeline

Stereo Cameras
→ Stereo Rectification
→ Depth Estimation
→ CNN Decision (Left / Right / Up / Down)
→ Operator Approval
→ MAVLink Command
→ Pixhawk Execution

All decisions and corrections are logged for continuous model improvement.

## Current Status

✅ Drone assembled
✅ Raspberry Pi ↔ Pixhawk MAVLink bridge established
✅ 3D stereo camera mount in design phase
⏳ Dataset collection in progress
⏳ CNN training phase upcoming

## 📡 Communication

MAVLink protocol for flight control

Waypoint setting from Raspberry Pi

Real-time telemetry feedback

Decision broadcasting for operator validation

## Roadmap
### Phase 1 – Stereo Vision

Camera synchronization

Depth estimation

Real-time disparity mapping

### Phase 2 – CNN-Based Decision System

Dataset labeling

Obstacle classification

Direction prediction model

### Phase 3 – Visual SLAM Integration

Landmark detection

Pose estimation

3D mapping

### Phase 4 – Assisted Autonomy

Human approval feedback loop

Model correction logging

### Phase 5 – Full Autonomy

Independent obstacle avoidance

Waypoint-based navigation

Autonomous mission execution

## Future Enhancements

Fisheye stereo SLAM

Infrared stereo for night navigation

Edge-optimized inference

Dynamic obstacle tracking

Real-time onboard 3D reconstruction
