# face-mask-detection-tensorflow
Developed an object detection system to identify and localize individuals wearing or not wearing masks using the TensorFlow Object Detection API

This project implements a real-time object detection system designed to identify and localize individuals wearing or not wearing masks. 

## Technical Overview
- **Framework:** TensorFlow.
- **Model Architecture:** Single Shot MultiBox Detector (SSD) with a MobileNet V2 backbone from the TensorFlow Model Garden.
- **Goal:** Identify, localize, and sort objects in new, unseen images.

## Dataset
[cite_start]This project utilizes the [Face Mask Detection Dataset](https://www.kaggle.com/datasets/andrewmvd/face-mask-detection) from Kaggle.
- **Total Images:** 853.
- **Annotations:** 853 XML files in PASCAL VOC format.
- **Classes:** `with_mask`, `without_mask`, and `mask_weared_incorrect`.

## Implementation Details
1. **Data Pipeline:** Developed a script to convert XML annotations into a structured Pandas DataFrame containing bounding box coordinates (`xmin`, `ymin`, `xmax`, `ymax`).
2. **Environment:** Built and executed using Google Colab with Google Drive integration for dataset management.
3. **Visualization:** Utilized the TensorFlow Object Detection API to overlay bounding boxes and class labels on test images.
