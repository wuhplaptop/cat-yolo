# Cat-50e-11n

## Model Overview

**Architecture:** YOLOv11  
**Training Epochs:** 50  
**Batch Size:** 32  
**Optimizer:** auto  
**Learning Rate:** 0.0005  
**Data Augmentation Level:** Moderate

## Training Metrics

- **mAP@0.5:** 0.98567

## Class IDs

| Class ID | Class Name |
|----------|------------|
| 0 | Cat |


## Datasets Used

- cat-2er75_v4
- cats-j6k8r-iakbs_v1
- cats-j6k8r_v1
- mickey-finder_v1

## Class Image Counts

| Class Name | Image Count |
|------------|-------------|
| Cat | 9147 |


## Description

This model was trained using the YOLOv11 architecture on a custom dataset. The training process involved 50 epochs with a batch size of 32. The optimizer used was **auto** with an initial learning rate of 0.0005. Data augmentation was set to the **Moderate** level to enhance model robustness.

## Usage

To use this model for inference, follow the instructions below:

```python
from ultralytics import YOLO

# Load the trained model
model = YOLO('best.pt')

# Perform inference on an image
results = model('path_to_image.jpg')

# Display results
results.show()
