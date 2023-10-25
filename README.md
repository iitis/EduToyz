# EduToyz

## Code and data for the paper 'Robust category recognition based on deep templates for educational mobile applications'

This repository contains data and programs that can be used to reproduce the results obtained for the article "Robust category recognition based on deep templates for educational mobile applications."

Below, we describe all the components of the repository:

* DATASET -  a folder with the EduToyz dataset. It contains various instances of 6 objects (items (toys) that could be used in the early. It includes 8 subfolders: a raw dataset (with no split) and folders for different splits used to perform Deep Template generation and testing for Deep Template Matching. Each subfolder includes 2 folders with the datasets: train (data used for template generation) and test (used for testing).
stages of education to engage early learners in educational activities).
* class_mapping.txt 
* dedicated_objects_recognition_based_on_templates.ipynb - jupyter-lab notebook, which can be used to replicate the results obtained for 
MobileNetV2 (https://keras.io/api/applications/mobilenet/#mobilenetv2-function), 
EfficientNetV2B0 (https://keras.io/api/applications/efficientnet_v2/#efficientnetv2b0-function),
and ResNetV2 (https://keras.io/api/applications/resnet/#resnet50v2-function) 
 models on our EduToyz dataset, depending on the declared number of samples to create templates and test their performance for different metrics/similarity measures. 


Necessary packages for Python:

* tensorflow 2.10.0
* pandas 1.5.2
* numpy 1.23.3
* scikit-learn 1.1.2
* scipy 1.9.1
* matplotlib 3.6.0
* seaborn 0.12.1