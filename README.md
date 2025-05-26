# Medical Imaging Project
---
## Project Overview
This project involves handling DICOM medical images, where the goal is to load, visualize, and perform tumor segmentation.

**Structure**
```

medical_images_project/
├── animation_gif/                          # Contains projections and gif from the MIP
├── 3d_slicer_photos/                       # Contains the screenshots of the 3d slicer
├── task2_data/                             # Contains the np arrays used as data inputfor task2
├── 1447                                    # Specifies intentionally untracked files that Git should ignore
│   └── 11_AP_Ax5.00mm/                     # Reference DICOM series
│   └── 11_AP_Ax5.00mm_ManualROI_Liver.dcm  # Segmented liver DICOM file
│   └── 11_AP_Ax5.00mm_ManualROI_Tumor.dcm  # Segmented tumor DICOM file
└── README.md                               
```
---  

**Warnings**  
Although task 2 is separate from task 1, they are sequentially related. That is to say, in order to execute task 2 without problems, the liver and tumor mask must be resliced in the same form as the original images and of type uint8. And in turn for the original images it is supposed that their visualization is already improved. Also the task2_data folder contains arrays with these requirements.

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

