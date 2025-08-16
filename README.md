# *Aedes* Detection with YOLOv11

## Overview
This repository contains a Google Colab Notebook and associated files for training a YOLOv11 object detection model to identify *Aedes* mosquitoes. The notebook walks through the complete workflow, including model training, validation, and running inference on new images.

## Features
 - Model Training: Utilizes the Ultralytics YOLOv11 framework to train a custom object detection model (yolo11n).

 - Validation: Includes scripts to validate the trained model's performance on a test set, calculating key metrics like mAP.

 - Inference: Demonstrates how to use the final trained weights to run predictions on a folder of new images.

 - Logging: Supports TensorBoard for monitoring training progress within the Colab environment.

## Sample Dataset

A labeled dataset in YOLO format is required.

[IMPORTANT] Download the dataset from [https://universe.roboflow.com/cpe313-mtad2/trapmos].

Once downloaded, unzip the dataset and upload this to Google Drive.

## Setup

Google Drive structure should look like this:

My Drive/
└── project_dir/
    ├── MAST_Cloudnet_notebook.ipynb
    ├── dataset/
    │   ├── data.yaml
    │   ├── images/
    │   └── labels/
    └── images/
        └── inference_image.jpg
## Usage
Open the notebook in Google Colab:
1. Navigate to project_dir in Google Drive.
2. Double-click on MAST_Cloudnet_colab_notebook.ipynb to open it with Google Colab.
3. Execute the cells in the notebook sequentially to perform the following steps:
    - Initialization: Installs and checks the Ultralytics environment.
    - Training: Trains the YOLO model. Training progress and logs will be saved to a runs/ directory within your Google Drive project folder.
    - Validation: Evaluates the best-performing model (best.pt).
    - Detection: Runs inference on your test images.


