# Melanoma Detection Assignment
> Project by Géraldine Bengsch (Third Upgrad Assignment) <br>
>
> This project uses multiclass classification model using a custom convolutional neural network in TensorFlow..
> - Which variables are significant in predicting the price of a house
> - How well the variables describe the price of a house
>
> The project contains:
> - Data Analysis notebook
> - A folder containing images used (Visualisations are my own, picture is from Unsplash)
> - The data set `train.csv`
> - The data dictionary `datainfo.txt`
> - Answers to the Subjective Questions in pdf format `SubjectiveQuestions.pdf`


## Table of Contents
* [General Information](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Contact](#contact)


  
## General Information
  

![Photo by <a href="https://unsplash.com/es/@smirnovalery?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Valeria Smirnova</a> on <a href="https://unsplash.com/s/photos/skin?utm_source=unsplash&utm_medium=referral&utm_content=creditCopyText">Unsplash</a>](img/valeria-smirnova-xEK8bas1vqI-unsplash.jpg)
  








- **General information:** 
Problem statement: To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.
- **Background:** 
A US-based housing company named Surprise Housing has decided to enter the Australian market. The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price. For the same purpose, the company has collected a data set from the sale of houses in Australia. 

- **Business problem:**
Aim is to model the price of houses with the available independent variables. This model will then be used by the management to understand how exactly the prices vary with the variables. They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns. Further, the model will be a good way for management to understand the pricing dynamics of a new market.

## Project Pipeline/Assignment Steps performed in the notebook

- Data Reading/Data Understanding → Defining the path for train and test images 
- Dataset Creation→ Create train & validation dataset from the train directory with a batch size of 32. Also, make sure you resize your images to 180*180.
- Dataset visualisation → Create a code to visualize one instance of all the nine classes present in the dataset 
### Model Building & training : 
- Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
- Choose an appropriate optimiser and loss function for model training
- Train the model for ~20 epochs
- Write your findings after the model fit. You must check if there is any evidence of model overfit or underfit.
- Chose an appropriate data augmentation strategy to resolve underfitting/overfitting 
### Model Building & training on the augmented data :
- Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model rescale images to normalize pixel values between (0,1).
- Choose an appropriate optimiser and loss function for model training
Train the model for ~20 epochs
- Write your findings after the model fit, see if the earlier issue is resolved or not?
### Class distribution: Examine the current class distribution in the training dataset 
- Which class has the least number of samples?
- Which classes dominate the data in terms of the proportionate number of samples?
- Handling class imbalances: Rectify class imbalances present in the training dataset with Augmentor library.
### Model Building & training on the rectified class imbalance data :
- Create a CNN model, which can accurately detect 9 classes present in the dataset. While building the model, rescale images to normalize pixel values between (0,1).
- Choose an appropriate optimiser and loss function for model training
- Train the model for ~30 epochs
- Write your findings after the model fit, see if the issues are resolved or not?



## Conclusions
Please see the notebook for more detailed insights.
1. `GrLivArea` is by far the most important predictor
2. The top variables are intuitive.
3. Lasso is the chosen model for the final model, because it creates a simple model with the top features.





## Technologies Used

![Python](https://img.shields.io/badge/Python-3.10-informational?style=flat&logoColor=white&color=2bbc8a)
![NumPy](https://img.shields.io/badge/NumPy-1.21.5-informational?style=flat&logoColor=white&color=2bbc8a)
![Pandas](https://img.shields.io/badge/Pandas-1.3.5-informational?style=flat&logoColor=white&color=2bbc8a)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.5.1-informational?style=flat&logoColor=white&color=2bbc8a)
![Seaborn](https://img.shields.io/badge/Seaborn-0.11.2-informational?style=flat&logoColor=white&color=2bbc8a)
![sklearn](https://img.shields.io/badge/Sklearn-1.0.2-informational?style=flat&logoColor=white&color=2bbc8a)
![statsmodels](https://img.shields.io/badge/statsmodels-0.13.1-informational?style=flat&logoColor=white&color=2bbc8a)
![scipy](https://img.shields.io/badge/scipy-1.8.0-informational?style=flat&logoColor=white&color=2bbc8a)
![Tensorflow](https://img.shields.io/badge/tensorflow-2.9.0-informational?style=flat&logoColor=white&color=2bbc8a)
![Keras](https://img.shields.io/badge/keras-1.8.0-informational?style=flat&logoColor=white&color=2bbc8a)
![Pillow](https://img.shields.io/badge/pillow-1.8.0-informational?style=flat&logoColor=white&color=2bbc8a)



## Contact
Created by [@GeriNZ](https://github.com/GeriNZ) - feel free to contact me! <br>
Student at UpGrad: *Master of Science in ML and AI* <br>
© 2022
