# Visualizing Convolutional Neural Networks 

## Quick start:
To get the code up and running you will need to install our dependencies, they are all contained in "requirements.txt". you will need your environment to be python version 3.10

## Navigation:
Our repo is organized in a way that we can hopefully eventually apply the code to different models/datasets, here is a breakdown of the directories:

**/Covid19-dataset:** This is the dataset of 317 images that we used

**/models:** this contains the models to be used, in our case it's just a single model named: "covid_vgg1.h5"

**/Output_Images:** this directory contains the outputs for each technique

**/visualization_techniques:** this directory contains sub folders correlating to each technique, inside each folder is a jupyter notebook.


# How to execute each jupyter notebook:

## CAM:
`visualization_techniques/cam/cov19_cam.ipynb`

Adapted and modified code from https://towardsdatascience.com/practical-guide-for-visualizing-cnns-using-saliency-maps-4d1c2e13aeca

Basic notebook that uses class activation maps to view all layers from the first 5 test image predictions. Outputed to the `Output_Images/cam` directory.

## Grad-Cam:
`visualization_techniques/gradcam/98-48-accuracy-using-transfer-learning-vgg.ipynb`

Credit to GPT-4 for helping me implement this.

Run the Cells from top to bottom, you can skip over cell 6 if you don't want to evaluate the model. This code takes 10 minutes to execute on my computer. Outputs the images to `Output_Images/gradcam`

## Grad-Cam++:
`visualization_techniques/gradcam++/cov19_grad-cam++.ipynb`

Implementation adapted from https://github.com/samson6460/tf_keras_gradcamplusplus

Notebook that implements the gradcam++ technique. Creates and outputs images for all layers in the first 5 predictions for each class. Output location: `Output_Images/gradcam++`

## LIME:
`visualization_techniques/lime/cov19_lime.ipynb`

Implementation adapted from https://towardsdatascience.com/interpreting-image-classification-model-with-lime-1e7064a2f2e5

Notebook that implements the lime technique. Creates and outputs images for the first 5 predictions in each class. Output location: `Output_Images/lime`


## Saliency Map:
`visualization_techniques/saliency_map/cov19_saliency_maps.ipynb`

Credit to GPT-4 for helping me implement this.

Run the Cells from top to bottom, you can skip over cell 6 if you don't want to evaluate the model. this code is pretty simple and executes pretty fast. Outputs the images to `Output_Images/saliency_map`

## SmoothGrad:
`visualization_techniques/smoothgrad/smoothgrad2.ipynb`

Credit to: https://github.com/PAIR-code/saliency/blob/master/Examples_core.ipynb, most of the code is from them.

Run the Cells from top to bottom, although be warned, this method took 6 hours to render the images to the output in `Output_Images/smoothgrad`