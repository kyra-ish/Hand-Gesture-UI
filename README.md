# Multimodal Hand Gesture Recognition System & User Interface

An active, high-performance computing pipeline designed to bridge human spatial hand kinematics with generative transformer networks in real time. This repository implements an object-oriented Python architecture that pre-processes incoming frame blocks, tracks anatomical keypoints, and structures coordinate arrays for conversational interfaces.

## 🛠️ System Architecture

The software is modularly structured across three distinct layers:
1. **Input Layer (Computer Vision):** Captures high-frequency video frames via OpenCV, executing color-space transformations (BGR to HSV) and boundary thresholding to isolate hand geometries from background noise.
2. **Translation Layer (Modular Abstraction):** Computes geometric Euclidean distances between segmented landmark arrays, converting spatial motions into standardized semantic token sequences.
3. **Generative Interface Layer:** Feeds parsed token strings directly into Large Language Model API endpoints to generate context-aware, screen-free user responses.

## 🚀 Key Engineering Implementations
* **Dynamic Matrix Tracking:** Manages continuous state tracking of matrix arrays to extract multi-dimensional coordinate fields from webcam streams at low latency.
* **OOP Code Discipline:** Built strictly using robust object-oriented patterns in Python to ensure reusable data classes, maintainability, and clear separation of concerns.
* **Asynchronous Execution:** Optimized pipeline execution boundaries to decouple frame capture frequency from textual API processing times, preventing runtime thread bottlenecks.

## 📁 Repository Blueprint
* `/src` — Core application source code tracking modules.
* `/config` — System configuration thresholds, tracking rules, and parameters.
* `main.py` — High-performance entry point executing the coordinate loop.
