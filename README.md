# Melanoma Detection

> A CNN-based model to accurately detect melanoma, a type of skin cancer that accounts for 75% of skin cancer deaths. This solution evaluates images and alerts dermatologists about the presence of melanoma, potentially reducing manual diagnostic effort.

## Table of Contents
- [Problem Statement](#problem-statement)
  - [Business Understanding](#business-understanding)
  - [Business Goal](#business-goal)
  - [Business Risk](#business-risk)
- [Project Pipeline](#project-pipeline)
- [Technologies Used](#technologies-used)
- [Acknowledgements](#acknowledgements)
- [Contact](#contact)

## Problem Statement

### Business Understanding

The dataset consists of 2,357 images of malignant and benign oncological diseases from the International Skin Imaging Collaboration (ISIC). The images are classified into multiple disease categories with melanomas and moles slightly dominant.

The dataset includes the following diseases:
- Actinic keratosis
- Basal cell carcinoma
- Dermatofibroma
- Melanoma
- Nevus
- Pigmented benign keratosis
- Seborrheic keratosis
- Squamous cell carcinoma
- Vascular lesion

### Business Goal

To build a multiclass classification model using a custom convolutional neural network (CNN) in TensorFlow to classify skin diseases.

### Business Risk

- Incorrect classification of skin cancer poses significant health risks.

## Project Pipeline

1. **Data Reading/Data Understanding**: Define the path for train and test images.
2. **Dataset Creation**: Create train & validation datasets with a batch size of 32. Resize images to 180x180.
3. **Dataset Visualization**: Visualize one instance of each of the nine classes present in the dataset.
4. **Model Building & Training**: 
   - Build a CNN model to detect the 9 classes. Normalize pixel values (0,1).
   - Choose an optimizer and loss function.
   - Train for ~20 epochs, checking for overfitting or underfitting.
5. **Data Augmentation**: Apply augmentation to resolve overfitting/underfitting.
6. **Class Distribution**: Examine class distribution, identifying the least and most dominant classes.
7. **Handling Class Imbalances**: Use the Augmentor library to address class imbalances.
8. **Final Model Training**: Train the model for ~30 epochs on the augmented and balanced data. 

## Technologies Used
- `pandas` - 1.3.4
- `numpy` - 1.20.3
- `matplotlib` - 3.4.3
- `seaborn` - 0.11.2
- `plotly` - 5.8.0
- `sklearn` - 1.1.2
- `statsmodel` - 0.13.2
- `tensorflow` - 2.11.0

## Acknowledgements
- This project was developed as part of a group case study.
- Resources:
  - [GeeksforGeeks](https://www.geeksforgeeks.org/)
  - [Seaborn](https://seaborn.pydata.org/)
  - [Plotly](https://plotly.com/)
  - [Pandas](https://pandas.pydata.org/)
  - [TensorFlow](https://www.tensorflow.org/)

## Contact
Created by [@darshil2848] - feel free to contact me!
