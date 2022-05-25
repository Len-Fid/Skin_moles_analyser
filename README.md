<h2><p align="center"> Building a deep learning model that classifies the types of moles </p></h2>
<p align="center"><img src="https://cdn11.bigcommerce.com/s-o4p6cu3wts/images/stencil/original/uploaded_images/melanoma-skin-cancer.jpg?t=1589626592" width="500" height="300"></p>

## Description

**This is a learning project that involved data preprocessing and modelling used for computer vision using Tensorflow.**

### Dataset: 
For this project the [HAM10000("Human Against Machine with 10000 training images")](https://https://www.kaggle.com/datasets/kmader/skin-cancer-mnist-ham10000) dataset was used. This dataset consists of 10015 photos of 7 types of skin lesions. These involve both malignant and benign skin lesions. 

<p align="left"><img src="https://raw.githubusercontent.com/Len-Fid/Skin_moles_analyser/main/assets/download.png" width="350" height="450"></p>

### Strategy: 
* Due to the technical problems with the installation of Tensorflow on my computer, I switched to using Google Colab.
* Loaded the data from Kaggle directly to my Google Colab notebook. For the purpose of this project I used metadata.csv file. 
* Pre-processed the data using Pandas and Numpy. 
* Created the visualisations to understand the data better:
<p align="left"><img src="https://raw.githubusercontent.com/Len-Fid/Skin_moles_analyser/main/assets/graphs..JPG" width="400" height="300"></p>

* It is clear that we are faced with a very imbalanced data. Approximately 67% of all photos belong to one class ('nv': 'Melanocytic nevi)
* I explored different methods to tackle the imbalanced dataset.
  - Creating fake images with ImageDataGenerator (tf.keras.preprocessing) (upsampling everything or just the minority classes)
  - Upsampling and downsampling the dataset
  - Putting different weights on minority classes
* After understanding how data augmentation techniques work, I moved on to splitting my dataset
* I looked at different models and their advantages and setbacks 
* I opted out for MobileNet as my base model and Sequential()
* I have studied what does adding different layers does and how it affects the model 
* Due to the time limit, I didn't get to tune my model, so the accuracy is only 65%
* I struggled to deploy my model in Flask, because I don't have the libraries installed on my computer 

### Languages and libraries used:
**Python**:
  - Pandas 
  - Numpy 
  - Scikit-learn
  - Pillow 
  - MatPlotLib
  - Seaborn
  - Scipy
  - Autokeras

**Html** ( to prepare the templates for the deployment

### This is a work in progress
