# Home-Price-Prediction
Home Price Prediction using Linear Regression#2

This repository contains code for House Price prediction using Linear Regression. This project is based on the dataset that can be found through online.who has done a very excellent job in the area of AI and ML. The current repository contains a detailed description of the process of visualization and preprocessing the dataset. This repository also contains a stable version of Linear Regression that can be used in other projects related to Machine Learning

Table of Contents

Requirements
Training Linear Regression
Performance
Reference

Dataset and pre-processing

We currently provided the dataset in the directory ./dataset. However, the linear regression package can be used with various dataset.

Your data directory looks like:
(Optional) You can change the directory of the dataset when running the home.py in terminal.
- dataset/
    - __init__.py
    - dataset.py
    - config.py
    - divar_tehran_dataset ...
        - DivarHousePrice.csv
     
Training Linear Regression

We assume that you have cloned the repository.
To train Linear Regression using the terminal environment, we assume that the dataset is placed in ./dataset/divar_tehran_dataset/, so you should simply run the following command. !python train.py By running the following command, you will get more information about the module.
>!python train.py -help 
Usage: home.py [options]
Options:
  -h, --help            show this help message and exit
  -p TRAIN_PATH, --path=TRAIN_PATH
                        Path to training data.
  -m METHOD, --method=METHOD
                        choose between 'normal-equation' and 'gradient-descent'
                        default value is 'normal-equation'
As you can see above, you can choose either Linear Regression to be based on Gradient Descent or Normal Equation. However, the default method would be "normal-equation".

!python train.py -p "./dataset/divar_tehran_dataset/DivarHousePrice.csv" -m "gradient-descent"
training_process_GD.gif


Colaboratory Notebook

The Second way to train Linear Regression is to use the .ipynb file in the main directory. It is very informative and builds up your intuition of the process of pre-processing and makes you more knowledgeable about the dataset. In addition, you don't even need to clone the repository, because it can be executed by Google Colaboratory Online.


notebook_visualize.gif

References:

The following list contains several links to every resource that helped us implement this project.

Kaggle dataset published by Soheil Tehranipour
Maths-ML developed by Dhivya M
Machine Learning course published by Coursera
