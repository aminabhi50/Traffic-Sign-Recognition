# Traffic-Sign-Recognition (v1.0)
![GitHub followers](https://img.shields.io/github/followers/aminabhi50?style=social)![languages](https://img.shields.io/github/languages/count/aminabhi50/Traffic-Sign-Recognition)

Traffic sign recognition is the most popular topic of computer vision and deep learning in recent years. I choose this topic for my Research Methodology subject. The deep learning-based method, a custom convolutional neural network used for traffic sign recognition, classifies and recognizes 43 different traffic signs.

## Description
Nowadays, due to the rapid development of technology, autonomous vehicles are in trend at present. So, the Advanced Driver Assistance System (ADAS) is an important development for Intelligent Transportation System (ITS), and ADAS is one of the most important functions for autonomous vehicles. As a result, the Traffic Sign Recognition method is very promising for the development of ADAS, as well as it can be useful to reduce road mortality, as the system recognizes the traffic signs, and these recognized images are very helpful while driving vehicles.

Traffic Sign Recognition System is a vision-based system that can detect and recognize all traffic signs, even these signs are partially visible or distorted. For the implementation of traffic sign recognition, the deep learning-based method, a custom CNN was used. A custom CNN consists of 8 - Convolution layers, 4 - Max Pooling Layers, 4 - Dropout Layers, and 1 - Flatten layer to flatten the output of 4 - blocks, 2 - Fully Connected Layers, and finally, there is 1 - Output Layer having Softmax as an activation function. All other layers except the Output layer have a ReLU activation function. After training the model, I achieved 99.98% training accuracy and 97.60% testing accuracy.

## Custom CNN Architecture
![Architecture of Custom CNN](/images/CNNArchitecture.png)

## System Flow
![Flow Diagram](/images/FlowDiagram.png)

## Getting Started

### Dependencies
* **Required Libraries:** OpenCV, Numpy, Pandas, OS, Tensorflow, Keras, Sklearn, Matplotlib
* **Language:** Python above 3.5
* **Hardware Requirements:**
  * **RAM:** Approximately 8-10GB
  * **Disk Storage:** 1GB
  * **GPU Requirement**: Yes
* **Use Google Colab environment if possible as it provides all dependecies mentioned above with decent GPU**

### Manifest
```
RM_Project_PreprocessDataset_GTSRB.ipynb / RM_Project_PreprocessDataset_GTSRB.py :

  * Code to unzip the dataset folder
  * Code to load train and test images from the train and test folders with their labels information
  * Code to resize the images into 32x32 pixels
  * Code to store resized images data and class labels into separate Numpy files on Google Drive

RM_Project_GTSRB.ipynb / RM_Project_GTSRB.py :

  * Code to load resized images data and class labels from Numpy files
  * Code to train custom CNN model with loaded training and testing data.
  * Code to display classification report and confusion matrix for custom CNN model
  
images: This folder contains images of flow diagram, the architecture of CNN model, and sample images of dataset.

results: This folder contains images of experiment results that include accuracy and loss curves, classification reports, and confusion matrix.
```

### Dataset
#### German Traffic Sign Recognition Benchmark (GTSRB)
The dataset used can be downloaded here - https://www.kaggle.com/meowmeowmeowmeowmeow/gtsrb-german-traffic-sign

This dataset is an image classification dataset, which consists of 51839 images belonging to 43 different traffic signs with unbalanced class frequencies, having varying light conditions and rich backgrounds, and image sizes vary between 15x15 to 250x250 pixels:

**Training Data :** 39209 images <br/>
**Testing Data :** 12630 images

![Sample images of GSTRB Dataset](/images/GSTRB.png)

### Executing Program
There are mainly two ways to run the project:

**Method 1: Using Google Colab Environment**
* First, download the dataset from the given link and upload it on the drive. After that, download the RM_Project_PreprocessDataset_GTSRB.ipynb and RM_Project_GTSRB.ipynb, then first run RM_Project_PreprocessDataset_GTSRB.ipynb to resize the dataset, after that run RM_Project_GTSRB.ipynb to train and evaluate model.

**Method 2: Using Local Machine having decent GPU**
* First, download the dataset from the given link and store it at the appropriate location in your local machine. After that, download all necessary dependencies mentioned above and .ipynb or .py files. Then, change all the paths in code according to your local machine and run the RM_Project_PreprocessDataset_GTSRB.ipynb to resize the dataset, after that run RM_Project_GTSRB.ipynb to train and evaluate the model.

### Results
All images of experimental results that include accuracy and loss curves, classification report, and confusion matrix, are available in the [Results](/results/) folder. For more description of results images, please visit [Description of Results Images](/results/results_info.md).
 
## Authors
Abhi Amin <br/>
To contact send an email to (aminabhi50@gmail.com)

## Version History
* 1.0 - Final Release

## License
This project is open source.

## Project Status
The project is completed, but one can modify it by adding image preprocessing techniques such as data augmentation, and more layers to custom CNN model, to achieve better performance.
