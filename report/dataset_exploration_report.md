# Dataset Exploration Report for IrisCrypt

## Title
Exploration of the CASIA Iris Database for Secure Iris Biometric Authentication

---

## Introduction

In this project, I am developing a secure iris biometric authentication system called IrisCrypt. Before building the recognition model, it is important to understand the dataset that will be used for training and testing. For this purpose, I explored the CASIA Iris Database, which is one of the most widely used public datasets for iris recognition research.

This report summarizes the structure, characteristics, and observations made during the exploration of the dataset.

---

## Objective of Dataset Exploration

The main objectives of this dataset exploration are:

1. To understand the structure of the CASIA Iris Database.
2. To determine the number of subjects and images.
3. To examine the image format and resolution.
4. To visualize sample iris images.
5. To identify preprocessing requirements.
6. To confirm that the dataset is suitable for the IrisCrypt project.

---

## Dataset Source

- Dataset Name: CASIA Iris Thousand
- Source: Chinese Academy of Sciences Institute of Automation (CASIA)
- Type: Near-Infrared (NIR) Iris Images
- Number of Subjects: 2,000
- Approximate Number of Images: 20,000
- File Format: JPG
- Image Resolution: 640 × 480 pixels

---

## Dataset Folder Structure

After downloading and extracting the dataset, the folder structure is organized as follows:

IrisCrypt/
└── data/
    └── CASIA/
        └── CASIA-Iris-Thousand/
            ├── 001/
            ├── 002/
            ├── 003/
            └── ...

Each numbered folder represents one subject, and each folder contains multiple iris images of the left and right eyes.

---

## Dataset Characteristics

### Number of Subjects
The dataset contains 2,000 unique subjects.

### Number of Images
Each subject has multiple iris images, resulting in approximately 20,000 total images.

### Image Type
All images are grayscale near-infrared images, which reduce the effect of illumination and reveal clear iris texture.

### Variations Present
The dataset includes natural variations such as:

- Pupil dilation
- Eyelid and eyelash occlusion
- Reflection noise
- Slight gaze changes

---

## Exploration Performed

During Week 1, I performed the following tasks:

1. Downloaded the CASIA Iris Thousand dataset.
2. Extracted the dataset into the `data/CASIA/` folder.
3. Loaded the dataset using Python.
4. Counted the total number of subject folders.
5. Visualized sample iris images using Matplotlib.
6. Examined image dimensions and file format.
7. Saved screenshots of the results in the `results/week1_results/` folder.

---

## Sample Observations

After exploring the dataset, I observed the following:

- The dataset is well organized and easy to use.
- Iris patterns are clearly visible in most images.
- Images are consistent in size and format.
- Some images contain reflections and occlusions.
- Near-infrared imaging provides high contrast and clear texture details.

---

## Why I Selected the CASIA Dataset

I selected the CASIA Iris Database for the following reasons:

1. It is one of the most widely used iris recognition datasets.
2. It contains a large number of subjects and images.
3. The image quality is high.
4. It is commonly used in academic research.
5. It is suitable for both classical and deep learning-based approaches.

---

## Preprocessing Requirements

Based on the exploration, the following preprocessing steps will be required:

1. Image resizing
2. Contrast enhancement
3. Noise reduction
4. Iris segmentation
5. Normalization
6. Data augmentation (if necessary)

---

## Relevance to IrisCrypt

The CASIA Iris Database is highly suitable for the IrisCrypt project because it provides a large and diverse set of high-quality iris images. These images will be used to train and evaluate the ResNet-18 feature extraction model and to test secure template encryption and matching.

---

## Challenges Identified

Some challenges observed during exploration include:

- Reflections in the eye region
- Eyelash occlusion
- Pupil size variation
- Slight image blur

These issues will need to be addressed during preprocessing and segmentation.

---

## Conclusion

From the dataset exploration, I confirmed that the CASIA Iris Thousand dataset is well structured, large in size, and contains high-quality iris images suitable for biometric research. The dataset provides sufficient variation to develop and evaluate a secure iris authentication system. Based on this analysis, I conclude that the CASIA Iris Database is an excellent choice for implementing the IrisCrypt project.

---

## References

1. CASIA Iris Database, Chinese Academy of Sciences Institute of Automation.
2. John Daugman, "How Iris Recognition Works", 2004.