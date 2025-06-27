SOC_2025: Diabetic Retinopathy Image Processing

Overview

This repository contains code and documentation for a Summer of Code (SOC) 2025 project focused on computer vision for diabetic retinopathy (DR) detection. The project enhances retinal fundus images to improve the visibility of DR signs—microaneurysms (MAs), hemorrhages, exudates, and damaged blood vessels—using image processing techniques in Python with OpenCV, scikit-image, PyWavelets, and TensorFlow. It builds on concepts from the OpenCV Course - Full Tutorial with Python and research by Nagpal et al. (2022). The project is implemented in Google Colab, leveraging its free GPU for efficient processing.

The repository includes:





Python Code: Two Google Colab notebooks for Week 3 (basic preprocessing) and Week 4 (advanced processing and detection).



LaTeX Documentation: Detailed reports (computer_vision_introduction.tex, diabetic_retinopathy_week4.tex, etc.) explaining the methodology, aligned with SOC 2025’s emphasis on innovative open-source contributions [Web ID: 0, 3].

Dataset

The dataset consists of 50 retinal fundus images (image001_lesion.png to image050_lesion.png) stored in /content/drive/MyDrive/SOC_2025/week3/example_images/. These RGB images contain potential DR signs, assumed to be annotated visually or via an external file (e.g., CSV, not included). Outputs are saved to /content/drive/MyDrive/SOC_2025/week3/advanced_images/.

Repository Contents

Code





Week 3 Notebook (week3_dr_processing.ipynb): Implements basic image processing:





Preprocessing: Gaussian blur and CLAHE for noise reduction and contrast enhancement.



Segmentation: HSV thresholding for MAs/hemorrhages, Lab color space for exudates, Frangi filter for vessels.



Output: Enhanced images saved as _enhanced.png.



Week 4 Notebook (week4_dr_advanced.ipynb): Extends Week 3 with:





Advanced Preprocessing: Optimized CLAHE and curvelet-based enhancement (PyWavelets).



Lesion Enhancement: Texture filtering for MAs, refined Frangi for vessels.



Automated Detection: Contour-based exudate detection, with optional CNN training (ResNet50) if annotations are available.



Output: Enhanced images (_advanced.png, _curvelet.png) and contour-marked images (_contours.png).



These files provide a comprehensive methodology, suitable for SOC 2025 project documentation.
