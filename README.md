Disaster Damage Assessment Using Semantic Change Detection and Deep Learning
Overview

This project implements an automated disaster damage assessment framework using deep learning techniques to detect and classify building damage from pre-disaster and post-disaster satellite or drone images. The system combines Siamese U-Net for semantic change detection with YOLOv8-Seg for building segmentation to produce GIS-compatible damage assessment reports for disaster response.

Workflow
Image acquisition from satellite or drone imagery
Image preprocessing (resize, normalization, alignment)
Semantic change detection using Siamese U-Net
Building segmentation using YOLOv8-Seg
Damage calculation using Intersection over Area (IoA)
Damage classification and GIS report generation
Damage Classification
Destroyed: > 70%
Major Damage: 25% – 70%
Minor Damage: 5% – 25%
Safe: ≤ 5%
Technologies Used
Python 3.8
PyTorch
YOLOv8 Segmentation
OpenCV
NumPy
Flask
GDAL
Rasterio
GeoPandas
Datasets
xBD Dataset
xView2 Dataset
Satellite Imagery
Drone Imagery
Features
Automated semantic change detection
Building footprint segmentation
Pixel-level damage estimation
GIS-compatible output
Color-coded damage visualization
Real-time disaster assessment
Supports earthquakes, floods, hurricanes, cyclones, and building collapse scenarios
Repository Structure
project/
│── model.py                # Siamese U-Net implementation
│── inference.py            # Prediction pipeline
│── app.py                  # Flask application
│── requirements.txt        # Project dependencies
│── project report.pdf      # Complete project documentation
│── project presentation.pptx # Project presentation
Installation

Install the required libraries:

pip install -r requirements.txt
Run the Project
python app.py
Output

The system generates:

Semantic change detection maps
Building segmentation masks
Color-coded damage visualization
Building-wise damage classification
GIS-compatible damage assessment reports
Summary statistics of affected structures
Future Improvements
Transformer-based models (SegFormer, Swin-UNet)
Integration of SAR imagery (Sentinel-1)
LiDAR-based 3D damage estimation
Real-time deployment on NVIDIA Jetson devices
Automated GIS dashboards
Predictive disaster intelligence and early warning systems
Project Documents
Project Report: project report.pdf
Project Presentation: project presentation.pptx
Authors:
Y. Ajay
G. Karthika
M. Vijaya
V. Praveen
