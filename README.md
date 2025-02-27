 Potato Disease Classification
This repository contains a project focused on classifying potato diseases using a convolutional neural network (CNN) model. The dataset used for this project is from Kaggle.

Table of Contents

Project Overview
Dataset
Setup Instructions
Prerequisites
Installing Dependencies
Dataset Preparation
Running the Notebook
Project Structure
Acknowledgements


Project Overview
The goal of this project is to develop a machine learning model that can classify potato leaves as healthy or diseased. The model is built using a convolutional neural network (CNN) and trained on a dataset of potato leaf images.

Dataset
The dataset is sourced from Kaggle and includes images of healthy potato leaves as well as leaves affected by various diseases. You can download the dataset from here.

Setup Instructions
Prerequisites
Make sure you have the following software installed:

Python 3.x
Jupyter Notebook

Installing Dependencies
Install the required Python libraries using pip:

pip install tensorflow matplotlib splitfolders

Dataset Preparation
Organize the dataset in the following structure:

data/
└── raw/
    └── PlantVillage/
        ├── Healthy/
        ├── Late_blight/
        └── Early_blight/

        
Use the splitfolders library to split the raw data into training, validation, and testing sets:

splitfolders --output data/dataset --ratio 0.7 0.1 0.2 -- data/raw/PlantVillage/
Running the Notebook
Clone this repository:

git clone https://github.com/yourusername/potato-disease-classification.git
cd potato-disease-classification


Open the Jupyter notebook:

jupyter notebook potato-disease-classification-model.ipynb
Run the cells sequentially to train and evaluate the model.

Project Structure

potato-disease-classification/
├── data/
│   ├── raw/
│   │   └── PlantVillage/
│   │       ├── Healthy/
│   │       ├── Late_blight/
│   │       └── Early_blight/
│   └── dataset/
│       ├── train/
│       ├── val/
│       └── test/
├── potato-disease-classification-model.ipynb
└── README.md
Acknowledgements

Dataset: PlantVillage on Kaggle
