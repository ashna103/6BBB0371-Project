# 6BBB0371 Project-2024
## **Muscle Fiber Cross-Sectional Area (CSA) Segmentation and Analysis Project**
## Project under Dr. Mark Holt comparing Manual vs ML based muscle CSA segmentation


## Project Overview

This project focuses on the segmentation and quantification of muscle fiber cross-sectional area (CSA) using manual and machine learning (ML) methods. The goal is to compare the effectiveness of traditional manual segmentation with ML-based segmentation methods, specifically those implemented in the Fiji image processing platform combined with WEKA, a machine learning toolkit. By evaluating both methods, the project aims to assess how ML algorithms can automate and enhance the accuracy of CSA measurements in skeletal muscle fibers.

## Objectives
1. Compare manual and ML-based segmentation techniques for CSA measurement.
2. Assess the impact of pre-processing techniques (e.g., Gaussian filter) on segmentation quality.
3. Evaluate the accuracy and efficiency of ML algorithms when applied to a variety of datasets.
4. Investigate the limitations of both manual and automated methods, particularly concerning biological feature recognition, noise reduction, and segmentation completeness.
5. Propose strategies for improving ML-based CSA quantification for biological and clinical applications.

## Methodology

### Data
- **Datasets:** Images of skeletal muscle fibers stained using immunohistochemistry techniques.
- **Segmentation Methods:** Both manual and automated (ML-based) segmentation methods were applied to multiple datasets.

### Pre-processing
Prior to segmentation, images were pre-processed to enhance feature recognition. A Gaussian filter was applied to some images to reduce noise, facilitating improved segmentation accuracy.

### Segmentation
Following pre-processing, the datasets were segmented using two primary methods:
1. **Manual Segmentation** – Performed by manually tracing muscle fibers using Fiji.
2. **Machine Learning-Based Segmentation** – Utilized the WEKA toolkit within Fiji, leveraging ML algorithms to automate segmentation and quantify muscle CSA.

### Analysis
- Comparison between manual and ML-based segmentation was made based on the following metrics:
  - **Accuracy** of CSA measurements
  - **Efficiency** in terms of time required for segmentation
  - **Consistency** across datasets
  - **Circularity values** were analyzed to gauge the quality of segmented fibers, with particular attention to variations in box plot heights, ranges, and median skew.

## Results
Key findings from the project include:
1. **Discrepancies in Segmentation**: The ML-based methods struggled with finer biological features, particularly in cases of image noise. However, applying a Gaussian filter significantly improved the accuracy of ML segmentation.
2. **Accuracy Improvements**: ML-based methods generally performed well, but further improvements in image quality and training are needed to match the precision of manual methods.
3. **Circularity Analysis**: The box plots of circularity values revealed significant differences between the segmentation methods, with ML-based unfiltered images displaying wider ranges of circularity (min: 0.59, max: 0.81), while the other methods were more consistent (range 0.7 to 0.8).

## Future Outlook
- Further improvements in the robustness of ML models across varying imaging conditions will enhance generalizability.
- Exploration of advanced ML techniques and novel approaches will likely improve accuracy and efficiency.
- Integration of ML-based CSA quantification tools into clinical workflows, such as radiology and physical therapy departments, could streamline muscle assessment and patient care.

## Requirements

- **Fiji** (ImageJ) with the WEKA plugin for machine learning-based segmentation.
- **Python** or **MATLAB** (optional) for additional data analysis.
- **Mathematica** for visualizing segmentation results (e.g., colorization based on index).

## How to Use

1. Pre-process images using Fiji's built-in tools (optional: apply Gaussian filter).
2. Perform segmentation using either the manual method (tracing muscle fibers) or the ML-based method (WEKA plugin).
3. Analyze the segmented CSA using Fiji’s measurement tools.
4. Optionally, visualize and compare results using the provided scripts or your own analysis tools.


