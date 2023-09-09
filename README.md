# Melanoma Detection Assignment
> To build a CNN based model which can accurately detect melanoma. Melanoma is a type of cancer that can be deadly if not detected early. It accounts for 75% of skin cancer deaths. A solution that can evaluate images and alert dermatologists about the presence of melanoma has the potential to reduce a lot of manual effort needed in diagnosis.


## Table of Contents
- [Melanoma Detection Assignment](#melanoma-detection-assignment)
  - [Table of Contents](#table-of-contents)
  - [General Information](#general-information)
  - [Conclusions](#conclusions)
  - [Technologies Used](#technologies-used)
  - [Acknowledgements](#acknowledgements)
  - [Contact](#contact)


## General Information
- The dataset consists of 2357 images of malignant and benign oncological diseases, which were formed from the International Skin Imaging Collaboration (ISIC). 
- All images were sorted according to the classification taken with ISIC, and all subsets were divided into the same number of images, with the exception of melanomas and moles, whose images are slightly dominant.
- The data set contains the following diseases:  
**Actinic keratosis**  
**Basal cell carcinoma**   
**Dermatofibroma**  
**Melanoma**  
**Nevus**  
**Pigmented benign keratosis**  
**Seborrheic keratosis**  
**Squamous cell carcinoma**  
**Vascular lesion**



## Conclusions
- CNN based model was built to detect melanoma.
- First model was built with 3 convolutional layers and 1 dense layer. The model was overfitting. To reduce overfitting, more images with augmentation were used. 
- Second model was built with 3 convolutional layers and 1 dense layer along with the augmented images. The model was able to handle overfitting. However the accuracy was not good.
- There was a class imbalance in the dataset. To handle this, augmentated images were used to balance the dataset such that each class has 500 images. This was achieved using Augmentor library.  
![class imbalance](https://github.com/robinsonrajan/Melanoma-Detection-Assignment/blob/main/CNN%20Readme%20Image/class%20imbalance.png)
- Third model was built with 3 convolutional layers and 1 dense layer along with the augmented images. The model was able to handle overfitting and the accuracy was good.  
![Training and Validation Accuracy](https://github.com/robinsonrajan/Melanoma-Detection-Assignment/blob/main/CNN%20Readme%20Image/Training%20and%20Validation%20loss.png)


## Technologies Used
- pathlib - 1.0.1
- tensorflow - 2.13.0
- seaborn - 0.12.2
- matplotlib - 3.7.1
- numpy - 1.23.5
- pandas - 1.5.3
- Augmentor-0.2.12

## Acknowledgements
- This assignment is part of the course Executive PG Programme in Machine Learning and Artificial Intelligence offered by UpGrad.
- The dataset is provided by UpGrad.


## Contact
Created by [@robinsonrajan] - feel free to contact me!
