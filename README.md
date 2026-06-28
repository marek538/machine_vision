This repository showcases three interesting projects developed as part of a Machine Vision course, demonstrating practical applications of image processing, perspective geometry, and spatial analysis.

# 1) Depth Map Spatial Analysis

## Problem
Identify the spatial relationships and relative distances of multiple objects using raw depth maps from RGBD/Time-of-Flight (ToF) sensors.

## Solution
Processed radiometric depth data by generating contour masks and analyzing pixel arrays to programmatically pinpoint the minimum and maximum depth values, accurately identifying the closest and farthest objects in the scene.

# 2) Perspective Geometry: Height and Distance Estimation

## Problem
Measure exact real-world distances and estimate the physical heights of objects from a single 2D image without a direct pixel-to-millimeter scaling factor, compensating for severe perspective distortion.

## Solution
Utilized Canny edge detection, Hough transform, and the RANSAC algorithm to dynamically locate vanishing points and the horizon line. Applied 2D perspective transformations (homography matrix) and projective geometry concepts (cross-ratio) to accurately map pixel coordinates to real-world metric dimensions.

# 3) Cylindrical QR Code Reader

## Problem
Read QR codes attached to rotating cylindrical surfaces (such as cans) captured by a line-scan camera, which introduces specific surface deformations and stretching.

## Solution
Utilized a YOLOv8-based detection model to locate and segment the QR code, applying the `pyzbar` library to successfully parse the encoded data despite the cylindrical distortion
