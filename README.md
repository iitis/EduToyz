Code and data for the paper 'Robust category recognition based on deep templates for educational mobile applications'

This repository contains data and programs that can be used to reproduce the results obtained for the article 
"Robust category recognition based on deep templates for educational mobile applications."

Below, we describe all the components of the repository:

* DATASET - a folder with two datasets: EduToyz and Imagenette.
EduToyz contains various instances of 6 objects (items (toys) that could be used in the early stages of education to engage early learners in educational activities). It includes 8 subfolders: a raw dataset (with no split) and folders for different splits used to perform Deep Template generation and  testing for Deep Template Matching. Each subfolder includes 2 folders with the datasets: train (data used for template generation) and  test (used for testing). 
* class_mapping.txt - a dictionary that can be used to map numerical labels of our classes to human-readable names 
* dedicated_objects_recognition_based_on_templates_with_EduToyz.ipynb and dedicated_objects_recognition_based_on_templates_with_Imagenette.ipynb - jupyter-lab notebook, each dedicated to work with one of the databases. With these notebooks it is possible to repeat experiments for: MobileNetV2 (https://keras.io/api/applications/mobilenet/#mobilenetv2-function), EfficientNetV2B0 (https://keras.io/api/applications/efficientnet_v2/#efficientnetv2b0-function), and ResNetV2 (https://keras.io/api/applications/resnet/#resnet50v2-function) models on our EduToyz dataset, depending on the declared number of samples to create templates and test their performance for different metrics/similarity measures. 

Besides EduToyz, we also use a freely available dataset - Imagenette - which is a subset of ImageNet (it can be found at https://www.tensorflow.org/datasets/catalog/imagenette). It is possible to select any objects from this dataset. However, it is required to prepare subfolders analogously to the EduToyz database. We selected objects with the following WordNet identifiers: n03425413, n03445777, n02979186, n03000684, n03394916 (which for simplicity we have named respectively: "gas_station", "golf_ball", "radio", "chainsaw","instrument"), as they present object-like categories, which are the most suitable for our case. 

Necessary packages for Python:

* tensorflow 2.10.0
* pandas 1.5.2
* numpy 1.23.3
* scikit-learn 1.1.2
* scipy 1.9.1
* matplotlib 3.6.0
* seaborn 0.12.1