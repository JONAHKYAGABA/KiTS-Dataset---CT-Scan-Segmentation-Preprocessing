# KiTS-Dataset---CT-Scan-Segmentation-Preprocessing
KiTS Dataset - CT Scan Segmentation &amp; Preprocessing
This project provides a complete pipeline for processing and visualizing the KiTS (Kidney Tumor Segmentation) dataset. It includes CT scan preprocessing, segmentation mask alignment, orientation correction, slice-level PNG export, and train-validation-test splitting—ultimately preparing data for deep learning applications in kidney/tumor segmentation.
📊 Features
✅ Loads and processes 3D CT and segmentation NIfTI files

✅ Automatically reorients data to RAS+ canonical orientation

✅ Applies Hounsfield windowing for kidney-optimized view

✅ Converts axial slices into PNG images and masks

✅ Supports overlays with contour plots of segmented areas

✅ Splits data into Train / Validation / Test (customizable)

✅ Saves metadata and integrity verification plots
📊 Dataset Visualization
Orientation previews for kidney vs tumor per window (kidney, lung, soft tissue)

Distribution of slices per patient

Class distribution across slices using boxplots

Sample overlays and contour maps for inspection

✅ Verification
Each split is automatically verified:

Ensures masks and images are aligned

Confirms segmentation is present

Overlays are drawn and saved as visual debugging tools

📌 Notes
This script handles NIfTI to PNG preprocessing and segmentation mask overlay for semantic segmentation models.

The segmentation mask values are scaled to:

0: background

127: kidney

254: tumor

📚 References
KiTS19 Dataset

NiBabel
