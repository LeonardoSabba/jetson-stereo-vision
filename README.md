# Jetson Stereo Vision

A C++ stereo vision project using two Raspberry Pi cameras
connected to an NVIDIA Jetson.

## Objectives

- Capture images from two cameras.
- Synchronize the camera streams.
- Calibrate the stereo camera system.
- Rectify the images.
- Calculate a disparity map.
- Estimate object distances.

## Technologies

- C++17
- OpenCV
- CMake
- NVIDIA Jetson
- Git
- GitHub

## Build

```bash
cmake -S . -B build
cmake --build build
