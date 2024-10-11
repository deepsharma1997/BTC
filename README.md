# Brain Tumor Classifier - BTC
The python notebooks contain the code for multi-class brain tumor classification using various DCNN archiectures.

## Table of Contents

1. [Overview](#overview)
2. [Getting Started](#getting-started)
    1. [Dependencies](#dependencies)
    2. [Installation](#installation)
3. [Project](#project)
4. [Results](#results)
3. [Author](#author)

## Overview <a name="overview"></a>
In the current project, the capability of pre-trained Deep Convolutional Neural Network (DCNN) by ImageNet features is 
proposed for categorization of brain tumors by utilizing MR images. The pre-trained models like ResNet50, InceptionV3, 
Xception, DenseNet121, MobileNetV3Large, EfcientNetB0, EfcientNetV2L, EfcientNetV2B0 have been exploited for 
classifcation purpose.

## Getting Started <a name="getting-started"></a>

### Dependencies <a name="dependencies"></a>
* Python 3.×
* Libraries: NumPy, Pandas, Seaborn, Matplotlib, open-cv, Keras, tqdm, glob
* Google Colaboratory

### Installation <a name="installation"></a>

* Datasets: The dataset used in this project is publicly available and can be downloaded from Kaggle (https://www.kaggle.com/datasets/sartajbhuvaji/brain-tumor-classification-mri). It consists of 3264 brain MR images, which are subdivided  into 926 MR images of Glioma tumor, 937 MR images of  meningioma tumor, 901 MR images of pituitary tumor, and  500 MR images of no tumor.
* Colaboratory allows you to use and share Jupyter notebooks with others without having to download, install, or run anything on your own computer (other than a browser).

### Project  <a name="project"></a>

Brain tumors are the result of abnormal growth of cells and 
have dismal consequences on the patient’s body. The brain 
tumors are categorized on the pattern of cell development, 
which may be noncancerous in nature and are termed as 
benign, whereas the cancerous one is termed as malignant. 
Benign tumors propagate slowly, which do not spread and 
thus have no afect the associated normal brain parenchyma 
while malignant tumors growth is very rapid and afects 
other parts of brain.
* The algorithm is stated below.
* Input: List of images with supporting list of labels.
* Output: Trained model and predictions.
* Step1: Import all the images and labels into python lists.
* Step2: Resizing all the images to a size of 256*256.
* Step3: Converting all the resized images and supporting labels into NumPy arrays.
* Step4: Segregating the dataset into train & test sets and perform one-hot encoding on labels.
* Step5: Building the model:
* Step6: Compiling model by considering following 
parameters:
> Loss function=categorical_crossentropy.
- Optimizer=Adam.
- Performance metrics=Accuracy.
* Step7: Introduce callback functions used for metrics 
optimization.
- Tensor Board for measurements and visualizations of 
metrics.
- Model Checkpoint for check pointing the model weights.
- Reduce Learning Rate (LR) on plateau for reducing the 
learning rate for improving the metrics.
* Step8: Test the model and get predictions.

## Results<a name="results"></a>

In the end, I could validate a test image passed through the model.

![validation](https://github.com/nazianafis/Brain-Tumor-Classification/blob/main/screenshots/valid-img.png)

## Author<a name="author"></a>
* [Deepanshu Sharma](https://github.com/[deepsharma1997])


