# Automatic Classification of Good and Defective Bananas Using RGB Image Features and Naive Bayes Algorithm in Blawi Village, Lamongan Regency

## Abstract

Bananas are one of the most important agricultural commodities in Blawi Village, Karangbinangun District, Lamongan Regency, East Java. The quality of bananas significantly affects their market value, consumer acceptance, and distribution process. Traditional quality assessment is generally performed manually by farmers and traders based on visual observation, which can be subjective and inconsistent.

This research proposes an automatic banana quality classification system using Digital Image Processing and the Naive Bayes algorithm. The system extracts RGB color features from banana images and uses these features to classify bananas into two categories: Good Bananas and Defective Bananas. The objective of this study is to develop an intelligent classification model capable of assisting farmers and traders in assessing banana quality more accurately and efficiently.

Keywords: Banana Classification, Naive Bayes, Digital Image Processing, RGB Features, Machine Learning, Agricultural Informatics.

---


# Introduction

Agriculture plays an important role in supporting the economy of rural communities in Indonesia. Among various agricultural commodities, bananas are widely cultivated due to their high economic value and continuous market demand.

In Blawi Village, Karangbinangun District, Lamongan Regency, banana farming is one of the common agricultural activities. However, determining banana quality is still performed manually through visual inspection. This approach often leads to inconsistent results because it depends on human perception and experience.

Recent advances in Artificial Intelligence (AI), Machine Learning (ML), and Digital Image Processing provide opportunities to automate the quality assessment process. By analyzing color characteristics from banana images, machine learning models can classify bananas automatically and consistently.

---

# Research Background

Banana quality directly influences market price, consumer satisfaction, and post-harvest management. Good quality bananas generally exhibit bright yellow coloration and minimal physical defects, whereas defective bananas may show dark spots, discoloration, bruises, or over-ripeness.

Manual inspection has several limitations:

- Subjective assessment.
- Inconsistent decision making.
- Time-consuming inspection process.
- Dependence on human expertise.

To overcome these challenges, image-based classification systems can be developed using machine learning techniques.

This research focuses on extracting RGB color features from banana images and classifying them using the Naive Bayes algorithm.

---

# Problem Statement

The traditional banana quality assessment process in Blawi Village is performed manually and lacks consistency. There is a need for an intelligent system capable of automatically classifying banana quality based on image characteristics.

This study investigates whether RGB color features combined with the Naive Bayes algorithm can effectively distinguish between good and defective bananas.

---

# Research Objectives

The objectives of this research are:

1. To collect banana image data from Blawi Village.
2. To perform image preprocessing and RGB feature extraction.
3. To implement the Naive Bayes classification algorithm.
4. To classify bananas into Good and Defective categories.
5. To evaluate classification performance using standard metrics.
6. To develop a simple intelligent system for banana quality assessment.

---

# Research Questions

1. Can RGB image features be used to classify banana quality?
2. How effective is the Naive Bayes algorithm for banana classification?
3. What is the classification accuracy achieved by the proposed model?
4. Can the system assist farmers and traders in evaluating banana quality?

---

# Research Scope

This study focuses on:

- Banana images collected from Blawi Village.
- Two quality classes:
  - Good Banana
  - Defective Banana
- RGB color feature extraction.
- Naive Bayes classification algorithm.
- Evaluation using classification metrics.

The study does not include:

- Deep learning models.
- Texture feature extraction.
- Real-time camera integration.
- Multi-class banana maturity classification.

---

# Study Area

## Location

**Blawi Village**

District:
Karangbinangun

Regency:
Lamongan

Province:
East Java

Country:
Indonesia

Blawi Village is known for agricultural activities, including banana cultivation. The village provides an appropriate case study for investigating image-based banana quality classification.

---

# Dataset Description

The dataset consists of banana images divided into two categories:

## Good Bananas

Characteristics:

- Bright yellow color.
- Minimal defects.
- Fresh appearance.
- Suitable for sale and consumption.

## Defective Bananas

Characteristics:

- Black spots.
- Brown discoloration.
- Bruises.
- Overripe appearance.
- Physical damage.

Dataset Structure:

```text
dataset/
│
├── Banana_Good/
│   ├── image1.jpg
│   ├── image2.jpg
│   └── ...
│
└── Banana_Bad/
    ├── image1.jpg
    ├── image2.jpg
    └── ...
```

---

# Research Methodology

The research methodology consists of several stages:

## 1. Data Collection

Banana images are collected from local farmers, traders, and agricultural products in Blawi Village.

## 2. Data Preprocessing

Image preprocessing includes:

- Image loading.
- Image resizing.
- Noise reduction.
- RGB color extraction.

## 3. Feature Extraction

The system extracts:

- Mean Red (R)
- Mean Green (G)
- Mean Blue (B)

These values become input features for classification.

## 4. Dataset Preparation

The extracted features are stored in a structured dataset.

Example:

| Mean_R | Mean_G | Mean_B | Label |
|---------|---------|---------|---------|
| 180 | 165 | 80 | Good |
| 120 | 100 | 60 | Bad |

---

# Image Processing Techniques

Digital image processing is used to transform raw images into numerical data.

The process includes:

1. Reading image files.
2. Converting images into RGB arrays.
3. Calculating average color intensity.
4. Generating feature vectors.

RGB features are selected because banana quality is strongly associated with color changes during ripening and deterioration.

---

# Naive Bayes Classification

Naive Bayes is a probabilistic machine learning algorithm based on Bayes' Theorem.

Advantages:

- Simple implementation.
- Fast training process.
- Effective for small datasets.
- Low computational requirements.

In this study, Gaussian Naive Bayes is used because RGB values are continuous numerical variables.

---

# Experimental Workflow

```text
Banana Image Collection
            ↓
Image Preprocessing
            ↓
RGB Feature Extraction
            ↓
Dataset Creation
            ↓
Training and Testing Split
            ↓
Naive Bayes Training
            ↓
Prediction
            ↓
Performance Evaluation
            ↓
Banana Quality Classification
```

---

# System Architecture

```text
Input Banana Image
          ↓
Image Processing Module
          ↓
RGB Feature Extraction
          ↓
Feature Dataset
          ↓
Naive Bayes Model
          ↓
Prediction Result
          ↓
Good Banana / Defective Banana
```

---

# Evaluation Metrics

The classification model is evaluated using:

## Accuracy

Measures overall classification correctness.

## Precision

Measures prediction reliability.

## Recall

Measures the model's ability to identify actual positive samples.

## F1-Score

Balances Precision and Recall.

## Confusion Matrix

Provides detailed classification results.

---

# Results and Discussion

The expected output includes:

- Classification accuracy.
- Confusion matrix visualization.
- Precision, Recall, and F1-Score.
- Comparison between actual and predicted labels.

The model is expected to demonstrate satisfactory performance in distinguishing good bananas from defective bananas based on RGB image features.

---

# Practical Applications

The proposed system can be used for:

- Farmer assistance systems.
- Agricultural quality control.
- Post-harvest management.
- Banana sorting automation.
- Agricultural decision support systems.

---

# Future Development

Future improvements may include:

1. Texture feature extraction.
2. HSV color space analysis.
3. Convolutional Neural Networks (CNN).
4. Mobile application implementation.
5. Real-time camera integration.
6. Multi-class maturity classification.
7. Cloud-based agricultural monitoring systems.

---


# Conclusion

This research proposes an automatic banana quality classification system using RGB image features and the Naive Bayes algorithm. By utilizing digital image processing techniques, the system can identify whether a banana belongs to the Good or Defective category. The study contributes to agricultural technology development in Blawi Village by providing an intelligent and objective method for banana quality assessment.

---

# Citation

If you use this project for research purposes, please cite:

Muhammad Afanul Mu'min. Automatic Classification of Good and Defective Bananas Using RGB Image Features and Naive Bayes Algorithm in Blawi Village, Lamongan Regency. 2026.
