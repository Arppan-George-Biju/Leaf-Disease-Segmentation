# Leaf Disease Spot Segmentation

## Digital Image Processing Mini Project

This project focuses on detecting and segmenting potential disease spots on tomato leaves using Digital Image Processing techniques.

## Problem Statement

Plant diseases can appear as visible spots or discolorations on leaves. Identifying these regions from leaf images can help in analyzing the affected areas. This project uses image segmentation techniques to separate potential disease-affected regions from tomato leaf images.

## Objectives

- To process tomato leaf images using Digital Image Processing.
- To convert RGB images into HSV color space.
- To detect potential disease spots using HSV thresholding.
- To improve the binary mask using morphological operations.
- To generate segmented disease spot images.
- To process multiple images automatically.

## Dataset

The project uses the Tomato Leaf Disease Detection dataset obtained from Kaggle.

The project uses 120 images from the Early Blight category.

Dataset source:

https://www.kaggle.com/datasets/kaustubhb999/tomatoleaf

The dataset images are color JPG images.

## Methodology

The project follows these main steps:

1. Image acquisition
2. RGB to HSV conversion
3. HSV thresholding
4. Binary mask generation
5. Morphological opening
6. Morphological closing
7. Bitwise masking
8. Disease spot segmentation
9. Batch processing of 120 images

## Technologies Used

- Python
- OpenCV
- NumPy
- Matplotlib
- Google Colab

## Project Structure

```text
Leaf-Disease-Segmentation/
│
├── code/
│   └── Leaf_Disease_Spot_Segmentation.ipynb
│
├── requirements.txt
│
└── README.md

Results

The system generates:

Binary masks representing detected potential disease regions.
Segmented images showing the detected regions on the original leaf images.

The project processes all 120 selected Early Blight images.

Limitations

The segmentation uses fixed HSV threshold values. Changes in lighting, leaf color, background, and disease appearance can affect the segmentation results.

The dataset does not provide pixel-level ground-truth masks for the selected images. Therefore, the results are evaluated mainly through visual comparison and parameter analysis rather than numerical segmentation metrics such as IoU or Dice score.

Future Scope

The project can be improved by using:

Adaptive thresholding
Color normalization
More diverse field images
Manually created ground-truth masks
Quantitative evaluation using IoU and Dice score
Advanced image segmentation and deep learning techniques
Conclusion

This project demonstrates how basic Digital Image Processing techniques can be used to segment potential disease spots from tomato leaf images. HSV thresholding combined with morphological operations provides a simple and understandable approach for leaf disease spot segmentation.