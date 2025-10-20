# Lyft-LIDAR-Autonomous-Driving-Object-Classification

## Overview
This project focuses on 3D object classification using LiDAR point cloud data from the Lyft Level 5 autonomous driving dataset. It provides scripts and tools for data loading, preprocessing, visualization, and building classification models to identify objects like vehicles, pedestrians, and cyclists in autonomous vehicle environments.

## Features
* Data handling with the official Lyft dataset SDK
* Advanced geometry utilities for 3D point cloud manipulation
* Rich visualization using Matplotlib, Plotly, Seaborn, PIL, and OpenCV
* Performance evaluation through sklearn metrics
* Efficient iterable progress bars with tqdm
* Utility modules for file and system operations

## Installation

1. Install dependencies via pip or conda:

```bash
pip install pandas numpy matplotlib plotly seaborn opencv-python lyft-dataset-sdk scikit-learn pyquaternion tqdm  
```

## Usage

1. Load and explore Lyft dataset samples
2. Visualize sensor data and annotations
3. Train or evaluate object classification models
4. Generate reports and confusion matrices for performance insights

## Code Structure

1. Data processing and geometry: lyft_dataset_sdk, pyquaternion
2. Visualization: matplotlib, plotly, seaborn, cv2, PIL
3. Machine learning and metrics: sklearn.metrics
4. Utilities: os, glob, pickle, json, tqdm

## License
This project is open-source and available under the MIT License.