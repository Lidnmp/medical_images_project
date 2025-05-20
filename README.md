# Medical Imaging Project
---
## Project Overview
This project involves handling DICOM medical images, where the goal is to load, visualize, and perform tumor segmentation.

---

## Objective
DICOM Loading and Visualization
- Load and visualize DICOM images from the HCC-TACE-Seg dataset.
- Manage and rearrange image data based on specific DICOM headers.
- Create animations to visualize Maximum Intensity Projections of the imaging data.

Tumor segmentation
- Extract tumor mask bounding box and centroid.
- Create a semi-automatic tumor segmentation (either the bounding box or the centroid of the tumor).
- Assess the correctness of the algorithm, numerically and visually (Visualize both ground truth and tumor mask generated).

