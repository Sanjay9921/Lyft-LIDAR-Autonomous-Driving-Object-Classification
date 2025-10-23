# Lyft-LIDAR-Autonomous-Driving-Object-Classification

## Overview

This project investigates 3D object classification using LiDAR point cloud data from the Lyft Level 5 autonomous driving dataset. Detailed analyses are performed to visualize and compare bounding box attributes across multiple object classes, revealing structured spatial patterns, pronounced class separability, and realistic spatial properties. These insights support dataset quality assurance and inform robust model development for autonomous vehicle perception systems.

## Features

* Data handling via the official Lyft dataset SDK
* Advanced geometry utilities for 3D point cloud manipulation
* Rich visualization using Matplotlib, Plotly, Seaborn, PIL, and OpenCV
* Performance evaluation metrics via scikit-learn
* Efficient tqdm progress bars for large-scale analysis
* Data wrangling and utility routines leveraging Python's standard library

## Key Insights from Data Exploration

1. Spatial Patterns: Box centers (center_x, center_y, center_z) cluster in meaningful strata—vehicles align strongly with street lanes; non-vehicles cluster near sidewalk or road edges. Multimodal scene features and realistic outliers reflect real urban complexity.
2. Class Separability: Vehicle types (cars, trucks, buses) are well-separated from non-vehicle classes (pedestrian, cyclist) by their box widths, lengths, and heights. Buses and trucks consistently have the largest dimensions, while pedestrians and cyclists are smallest.
3. Distribution Realism: Width, length, and height distributions for each class reflect real-world expectations (e.g., bus length > car length > bicycle).
4. Outliers and Annotation Quality: Some outliers and multimodal shapes in the distributions suggest diversity in scenes, annotation standards, or rare events, all valuable for training robust models.

## Installation

1. Install dependencies via pip or conda:

```bash
pip install pandas numpy matplotlib plotly seaborn opencv-python lyft-dataset-sdk scikit-learn tqdm
```

2. Usage

* Load and explore Lyft dataset samples
* Visualize object properties and spatial distributions
* Train/evaluate object classification models using annotated features
* Generate interpretability reports and confusion matrices for benchmarking

## Code Structure

* Data processing and geometry: lyft_dataset_sdk, pyquaternion
* Visualization: matplotlib, plotly, seaborn, cv2, PIL
* Machine learning and evaluation: scikit-learn
* Utilities and system tools: os, glob, pickle, json, tqdm

## Credits and Citations

* https://github.com/lyft/nuscenes-devkit
* https://www.kaggle.com/code/tarunpaparaju/lyft-competition-understanding-the-data
* https://www.kaggle.com/gaborfodor/eda-3d-object-detection-challenge