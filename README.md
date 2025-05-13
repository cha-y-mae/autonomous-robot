# Autonomous Line-Following Robot 

An embedded systems project built using the NVIDIA JetBot platform to autonomously navigate a modular field by following a black line, handling intersections, detecting obstacles, and adapting to environmental conditions.

## Overview

This project was developed as part of the **ENGR – UH 3530 Embedded Systems** course at NYU Abu Dhabi. The robot leverages real-time computer vision and decision-making algorithms to mimic the RoboCupJunior Rescue Line competition.

## Objectives

- **Line Following**: Detect and follow a black line on a white modular surface.
- **Intersection Handling**: Detect green markers to perform left/right turns or U-turns.
- **Obstacle Detection**: Stop when objects are detected using image segmentation.
- **Red Line Detection**: Halt upon detecting stop markers.
- **Environmental Adaptation**: Maintain performance under dynamic lighting conditions.

## Tech Stack

- Python
- OpenCV
- NVIDIA JetBot (Jetson Nano)
- Jupyter Widgets
- HSV Segmentation
- Real-time Motor Control Logic

## Core Features

### 1. Image Processing
- Grayscale conversion
- CLAHE contrast enhancement
- HSV segmentation for green and red markers
- Morphological filtering and contour detection

### 2. Navigation Logic
- ROI-based black line detection
- PID-like motor control based on error from center
- Turn decisions based on green marker position

### 3. Obstacle Detection
- Contour analysis in upper image regions
- Halting mechanism triggered by object size thresholds

### 4. Feedback & Debugging
- Real-time display of binary masks and camera feed
- Widgets for visualization during testing

## Results

- Successfully demonstrated line-following, red line halting, and green intersection handling.
- Real-time performance achieved with low latency on Jetson Nano.
- Robust under varying lighting and surface textures.
- Modular code allows easy future upgrades (e.g., ML-based detection).

## Demo & Screenshots

<!-- Add GIF or images here -->
![Demo Video](path/to/image1.png)

## 👨‍💻 Team

- Chaimae Abouzahir 
- Abay Oralov 
- Vladislav Zapromyotov
- Will Mekvabidze
