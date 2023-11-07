# Paper name : Cascaded-Ensemble-of-Features-for-TB-detection
Ensemble learning method (LR and Deep NNs) for detecting Tuberculosis from Chest X-rays. 

# Project Name : Tuberculosis Detection Using Chest Radiographs

## Project Overview
This project is based on the paper titled "Exploiting Cascaded Ensemble of Features for the Detection of Tuberculosis Using Chest Radiographs." The goal of the project is to detect tuberculosis from chest X-ray images using an ensemble of Logistic Regression Classifiers with handcrafted features and Convolutional Neural Networks (CNNs) with features extracted using the Transfer Learning technique.

## Technologies
-	Machine Learning
-	Deep Learning
## Techniques
-	Image processing
-	Transfer Learning

## Processes
-	EDA
-	Data Wrangling
-	Data Visualization
-	Feature Extraction
-	Models Training
-	Models Ensembling
-	Validation

## Datasets

The project utilizes Kaggle datasets, including the Montgomery and Shenzhen datasets, which contain chest X-ray images for tuberculosis detection.
Dataset link - https://www.kaggle.com/datasets/kmader/pulmonary-chest-xray-abnormalities

## Implementation
The project was implemented using Kaggle Notebooks, taking the following major steps:

1. Image preprocessing: Reshaping images to uniform sizes (224x224), min-max normalization, and rotation-invariant augmentation.
2. Feature extraction: Two distinct feature extraction procedures, including hand-engineered and deep learning-based features.
	Hand-engineered features like HoG and LBP were taken from the X -ray images.

   ![HOG Feature visualization](https://github.com/aiotsir/Cascaded-Ensemble-of-Features-for-TB-detection/assets/56543279/a8cdcd31-3df9-4093-b399-8e882da60274)

   fig : HoG Feature visualized





   ![LBP feature visualization](https://github.com/aiotsir/Cascaded-Ensemble-of-Features-for-TB-detection/assets/56543279/7c1a84a1-b8f6-4d95-a0ba-24cf5a1b9e57)

   fig: LBP  Feature visualized


	Employed Inception Net, Dense Net and CheXNet deep learning neural networks to extract features. 
         
 ![inceptionv3](https://github.com/aiotsir/Cascaded-Ensemble-of-Features-for-TB-detection/assets/56543279/b1013532-8714-4e63-b1f3-a5bfb85442da)
fig: Inception Net used for Feature Extraction

 
 ![dense169_feat_model](https://github.com/aiotsir/Cascaded-Ensemble-of-Features-for-TB-detection/assets/56543279/cdb2edc0-3645-46dc-9028-620e44b78772)
fig : DenseNet 169

![ChexNet_model](https://github.com/aiotsir/Cascaded-Ensemble-of-Features-for-TB-detection/assets/56543279/2b36cd0f-6039-44f0-b6a8-dbb188bc024b)
fig: CheXNet



3. Feature selection: Applying feature selection and reduction procedures for the aggregation process.
4. Classifier training: Training a logistic regression classifier for hand-engineered features and a Receptive-Field-Aware neural network for deep learning-based features.

 ![tbClf](https://github.com/aiotsir/Cascaded-Ensemble-of-Features-for-TB-detection/assets/56543279/c896ad06-5123-46e9-91b6-cf9fd2d30a0e)

 fig: CNN used for classifying the features extracted using Deep Learning Models


5. Ensemble model: Combining probability scores from both feature extraction methods to create a feature vector for the final classifier.

## Included in the Repository

1. **Code**: The project's Python code is available in the repository.
2. **Data**: A sample dataset is provided for reference.
3. **Models**: Pre-trained models and saved model weights.
4. **Notebooks**: Jupyter notebooks used for the project.
5. **Documentation**: Supplementary documentation for further reference.



## Features

- Detection of tuberculosis from chest X-ray images.
- Combination of hand-engineered and deep learning-based features.
- High accuracy in tuberculosis detection.

## Result
The ensemble with the combination of Machine Learning and Deep Learning Model gave the best performance with 99% accuracy.

