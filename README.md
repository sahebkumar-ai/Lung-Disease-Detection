# COVID-19 Chest X-Ray Classification Using Machine Learning

## Project Overview

This project focuses on the automatic classification of chest X-ray images into four categories:

* Normal
* COVID-19
* Lung Opacity
* Viral Pneumonia

The objective is to assist in the early detection and diagnosis of respiratory diseases using image processing and machine learning techniques.

---

## Dataset

The project uses the **COVID-19 Radiography Dataset**, which contains chest X-ray images categorized into four classes:

| Class           | Description                |
| --------------- | -------------------------- |
| Normal          | Healthy chest X-ray images |
| COVID           | COVID-19 infected patients |
| Lung_Opacity    | Lung opacity abnormalities |
| Viral_Pneumonia | Viral pneumonia cases      |

Dataset Structure:

```
COVID-19_Radiography_Dataset/
│
├── Normal/
│   └── images/
├── COVID/
│   └── images/
├── Lung_Opacity/
│   └── images/
└── Viral_Pneumonia/
    └── images/
```

---

## Project Workflow

### 1. Data Collection

* Loaded chest X-ray images from dataset folders.
* Created a dataframe containing image paths and corresponding labels.

### 2. Data Visualization

* Displayed sample images from each disease category.
* Performed exploratory analysis to understand class distribution.

### 3. Feature Extraction

Two handcrafted feature extraction techniques were implemented:

#### Local Binary Pattern (LBP)

* Captures local texture information.
* Generates histograms representing texture patterns.

#### Histogram of Oriented Gradients (HOG)

* Extracts edge and shape-based features.
* Effective for medical image classification tasks.

---

## Machine Learning Models

The following classification algorithms were evaluated:

1. Logistic Regression
2. Decision Tree Classifier
3. Random Forest Classifier
4. Support Vector Machine (SVM)
5. K-Nearest Neighbors (KNN)
6. Naive Bayes
7. XGBoost Classifier

---

## Performance Evaluation

Each model was evaluated using:

* Accuracy
* Precision
* Recall
* F1-Score

Scikit-learn's classification report was used to generate detailed performance metrics for each disease class.

### Evaluation Metrics

#### Accuracy

Measures overall prediction correctness.

#### Precision

Measures how many predicted positive samples are actually positive.

#### Recall

Measures how many actual positive samples are correctly identified.

#### F1-Score

Harmonic mean of Precision and Recall.

---

## Visualization

The project includes:

* Sample X-ray image visualization
* F1-Score comparison plots
* Model-wise performance analysis
* Class-wise performance comparison

Grouped bar charts were used to compare F1-Scores across different machine learning models.

---

## Technologies Used

### Programming Language

* Python

### Libraries

* NumPy
* Pandas
* OpenCV
* Matplotlib
* Seaborn
* Plotly
* Scikit-learn
* TensorFlow
* Keras
* XGBoost
* scikit-image
* tqdm

---

## Installation

Clone the repository:

```bash
git clone https://github.com/yourusername/covid-xray-classification.git
cd covid-xray-classification
```

Install required packages:

```bash
pip install -r requirements.txt
```

---

## Running the Project

Update the dataset path:

```python
path = "COVID-19_Radiography_Dataset"
```

Run the notebook or Python script:

```bash
python main.py
```

---

## Results

The system successfully classifies chest X-ray images into four categories using handcrafted image features and multiple machine learning algorithms.

Comparative analysis shows the effectiveness of feature extraction techniques such as HOG and LBP in distinguishing COVID-19 and other lung diseases.

---

## Future Improvements

* Deep Learning based CNN models
* Transfer Learning using ResNet50, VGG16, DenseNet
* Data Augmentation
* Hyperparameter Optimization
* Explainable AI (Grad-CAM)
* Real-time clinical deployment

---
