# Literature Review Report for IrisCrypt

## Title
Secure Iris Biometric Authentication System using Deep Learning and Encryption

---

## Introduction

Biometric authentication is one of the most reliable ways to identify a person. Among different biometric traits such as fingerprint, face, and voice, iris recognition is considered one of the most accurate methods because the texture pattern of the iris is unique for every individual and remains almost unchanged throughout life.

In this internship project, I am developing a secure iris biometric authentication system called IrisCrypt. The main goal of this project is to combine iris recognition, deep learning, and encryption to build a system that can accurately identify a person while also protecting their biometric data. For this project, I am using the CASIA Iris Database and studying research papers related to iris recognition and biometric template security.

This literature review summarizes the important concepts and research papers that are relevant to my project and explains how my proposed work differs from and improves upon previous studies.

---

## Project Objectives

1. To understand the complete iris recognition pipeline.
2. To study secure biometric template protection techniques.
3. To explore the CASIA Iris Database.
4. To use ResNet-18 for automatic iris feature extraction.
5. To generate biometric templates from extracted features.
6. To encrypt templates before storing them.
7. To compare templates for user authentication.
8. To evaluate system performance using accuracy, FAR, FRR, and EER.

---

## Methods and Algorithms Used in My Project

### Dataset
- CASIA Iris Database
- EyeDentity dataset (optional)

### Image Processing
- OpenCV for preprocessing and image enhancement
- Normalization and resizing

### Deep Learning
- ResNet-18 using transfer learning
- PyTorch framework

### Security
- AES Encryption for secure template storage

### Matching
- Cosine Similarity or Euclidean Distance
- Threshold-based authentication

### Evaluation Metrics
- Accuracy
- False Acceptance Rate (FAR)
- False Rejection Rate (FRR)
- Equal Error Rate (EER)

---

## Proposed Work

1. Download and explore the CASIA Iris Database.
2. Preprocess the iris images.
3. Perform iris segmentation and normalization.
4. Use ResNet-18 to extract feature vectors.
5. Convert feature vectors into biometric templates.
6. Encrypt the templates using AES.
7. Store the encrypted templates securely.
8. Compare templates during authentication.
9. Make the authentication decision.
10. Evaluate recognition accuracy and security.

The main contribution of my project is that it combines deep learning-based iris recognition with encryption-based template protection in a single secure authentication framework.

---

# 1. How Iris Recognition Works (2004)

**Author:** John Daugman  
**Year:** 2004

## Research Objective
To present a complete and highly accurate iris recognition system.

## Methodology Used
1. Iris image acquisition
2. Segmentation using the Integro-Differential Operator
3. Normalization using the Rubber Sheet Model
4. Feature extraction using 2D Gabor Wavelets
5. IrisCode generation
6. Matching using Hamming Distance

## Dataset Used
Large operational datasets involving millions of comparisons.

## Algorithms Used
- Integro-Differential Operator
- Rubber Sheet Model
- 2D Gabor Wavelets
- IrisCode
- Hamming Distance

## Relevance to My Project
Provides the fundamental iris recognition pipeline.

---

# 2. Biometric Template Security (2010)

**Authors:** Anil K. Jain, Karthik Nandakumar, Arun Ross  
**Year:** 2010

## Research Objective
To study methods for protecting biometric templates against theft and misuse.

## Methodology Used
Analysis of security threats and survey of template protection techniques.

## Dataset Used
Survey-based work; not focused on a single dataset.

## Algorithms and Techniques Used
- AES Encryption
- Hashing
- Cancelable Biometrics
- Secure Sketches
- Fuzzy Commitment

## Relevance to My Project
Provides the theoretical basis for encrypting iris templates.

---

# 3. Deep Learning for Iris Recognition: A Review (2023)

**Authors:** Yimin Yin, Siliang He, Renye Zhang, et al.  
**Year:** 2023

## Research Objective
To review modern deep learning methods for iris recognition.

## Datasets Discussed
- CASIA Iris Database
- IITD Iris Database
- UBIRIS
- ND-IRIS

## Algorithms Used
- CNNs
- ResNet
- DenseNet
- U-Net
- Vision Transformers

## Relevance to My Project
Supports the use of ResNet-18 for automatic feature extraction.

---

## Comparison Between Research Papers and My Project

### My Proposed Project – IrisCrypt
- Dataset Used: CASIA Iris Database
- Deep Learning Model: ResNet-18
- Security Method: AES Encryption
- Matching Method: Cosine Similarity or Euclidean Distance
- Unique Contribution: Combines deep learning and encryption in one secure authentication system.

### Comparison Summary
- Daugman (2004) provides the classical recognition pipeline.
- Jain et al. (2010) provides the security framework.
- Yin et al. (2023) provides modern deep learning approaches.
- My project integrates all three ideas into one practical system.

---

## Overall Conclusion

From the papers that I studied, I learned that John Daugman's work provides the basic foundation of iris recognition, Jain et al. explain how biometric templates should be protected, and Yin et al. show that deep learning models such as ResNet significantly improve recognition performance. Based on these studies, I propose to develop IrisCrypt using the CASIA dataset, ResNet-18, and AES encryption to create a secure and efficient iris biometric authentication system.

---

## References

1. Daugman, J. (2004). How Iris Recognition Works.
2. Jain, A. K., Nandakumar, K., & Ross, A. (2010). Biometric Template Security.
3. Yin, Y., He, S., Zhang, R., et al. (2023). Deep Learning for Iris Recognition: A Review.
