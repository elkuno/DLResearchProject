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
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sit amet purus sem. Vivamus eu luctus elit. Morbi aliquet diam ligula, vitae consectetur sapien aliquet at. Quisque ac justo nisi. Ut sed arcu sed odio cursus luctus a at elit. Aliquam feugiat, erat in accumsan hendrerit, nibh turpis lobortis eros, ac accumsan nibh ligula sit amet leo. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Ut tristique dui in neque mollis gravida. Quisque ut nibh ante.

## Grad-Cam:
`visualization_techniques/gradcam/98-48-accuracy-using-transfer-learning-vgg.ipynb`

Credit to GPT-4 for helping me implement this.

Run the Cells from top to bottom, you can skip over cell 6 if you don't want to evaluate the model. This code takes 10 minutes to execute on my computer. Outputs the images to `Output_Images/gradcam`

## Grad-Cam++:
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sit amet purus sem. Vivamus eu luctus elit. Morbi aliquet diam ligula, vitae consectetur sapien aliquet at. Quisque ac justo nisi. Ut sed arcu sed odio cursus luctus a at elit. Aliquam feugiat, erat in accumsan hendrerit, nibh turpis lobortis eros, ac accumsan nibh ligula sit amet leo. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Ut tristique dui in neque mollis gravida. Quisque ut nibh ante.

## LIME:
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla sit amet purus sem. Vivamus eu luctus elit. Morbi aliquet diam ligula, vitae consectetur sapien aliquet at. Quisque ac justo nisi. Ut sed arcu sed odio cursus luctus a at elit. Aliquam feugiat, erat in accumsan hendrerit, nibh turpis lobortis eros, ac accumsan nibh ligula sit amet leo. Class aptent taciti sociosqu ad litora torquent per conubia nostra, per inceptos himenaeos. Ut tristique dui in neque mollis gravida. Quisque ut nibh ante.

## Saliency Map:
`visualization_techniques/saliency_map/cov19_saliency_maps.ipynb`

Credit to GPT-4 for helping me implement this.

Run the Cells from top to bottom, you can skip over cell 6 if you don't want to evaluate the model. this code is pretty simple and executes pretty fast. Outputs the images to `Output_Images/saliency_map`

## SmoothGrad:
`visualization_techniques/smoothgrad/smoothgrad2.ipynb`

Credit to: https://github.com/PAIR-code/saliency/blob/master/Examples_core.ipynb, most of the code is from them.

Run the Cells from top to bottom, although be warned, this method took 6 hours to render the images to the output in `Output_Images/smoothgrad`