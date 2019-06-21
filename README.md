# AI-for-S.E.A-Computer-Vision-Challenge

This repository is a submission for the Grab AI for S.E.A Computer Vision Challenge. 

## Update:
We re-run the previous submission on a kaggle kernel using a single Tesla P100 GPU and managed to improve our test set accuracy to 91% (up from 89%) in only 8 epochs (down from 10 epochs previously). The updated file is marked as [Updated] above.

## Getting Started

### Download the Data

We use a preprocessed dataset containing the Stanford Car dataset by classes folder. The dataset can be found here: https://www.kaggle.com/jutrera/stanford-car-dataset-by-classes-folder

the dataset includes:
1. images of cars by classes folder (car_data.zip)
2. annotation for the train dataset (anno_train.csv)
3. annotation for the test dataset (anno_test.csv)
4. names of the cars (names.csv)

We prepocess the dataset by adding transformations and normalization to both the training and test set.

### Dependencies
We use the standard PyTorch libraries as well as supporting libraries

### Model 
The model we use is a pretrained ResNet50 model from torchvision.models library.

### Model Reproducibility
We train the model on a single Tesla P100 GPU using kaggle kernel and managed to get a 91% accuracy on the test dataset on 8 epochs. We implement an automated model saving that can be used later to reproduce the model performance. The instructions are included in the [Updated] Stanford_Car_ResNet50.ipynb file.
