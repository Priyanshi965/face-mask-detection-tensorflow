# face-mask-detection-tensorflow
Developed an object detection system to identify and localize individuals wearing or not wearing masks using the TensorFlow Object Detection API

This project implements a real-time object detection system designed to identify and localize individuals wearing or not wearing masks. 

## Technical Overview
- [cite_start]**Framework:** TensorFlow[cite: 5, 21].
- [cite_start]**Model Architecture:** Single Shot MultiBox Detector (SSD) with a MobileNet V2 backbone from the TensorFlow Model Garden[cite: 6].
- [cite_start]**Goal:** Identify, localize, and sort objects in new, unseen images[cite: 8, 10].

## Dataset
[cite_start]This project utilizes the [Face Mask Detection Dataset](https://www.kaggle.com/datasets/andrewmvd/face-mask-detection) from Kaggle[cite: 13, 27].
- [cite_start]**Total Images:** 853[cite: 68].
- [cite_start]**Annotations:** 853 XML files in PASCAL VOC format[cite: 69].
- **Classes:** `with_mask`, `without_mask`, and `mask_weared_incorrect`.

## Implementation Details
1. [cite_start]**Data Pipeline:** Developed a script to convert XML annotations into a structured Pandas DataFrame containing bounding box coordinates (`xmin`, `ymin`, `xmax`, `ymax`)[cite: 84, 97, 110].
2. [cite_start]**Environment:** Built and executed using Google Colab with Google Drive integration for dataset management[cite: 29, 31].
3. [cite_start]**Visualization:** Utilized the TensorFlow Object Detection API to overlay bounding boxes and class labels on test images[cite: 14, 16].
