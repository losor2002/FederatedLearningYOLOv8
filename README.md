# Federated Learning YOLOv8

## Introduction

University project about Federated Learning, for the <i>Data Science and Machine Learning</i> course at University of Salerno.

## Authors

* **Lorenzo Sorrentino**   - [losor2002](https://github.com/losor2002)
* **Giovanni Borrelli**    - [GiovanniBorrelli](https://github.com/GiovanniBorrelli)
* **Lorenzo Scorzelli**    - [Revolt234](https://github.com/Revolt234)

## How to run

No installation is required.

By following the steps of the [DataAugmentation.ipynb](https://github.com/losor2002/FederatedLearningYOLOv8/blob/master/src/data_augmentation_pothole_identification.ipynb) notebook, you can decide of how much images you want to increase the dataset, and it will also automatically download the [Pothole Dataset](https://universe.roboflow.com/santosh-ie6yy/yolov8-seg-4ezhu/dataset/2) needed for doing augmentation techniques. Alternatively, you can already use the datasets in the "datasets" folder and run the [FederatedLearning.ipynb](https://github.com/losor2002/FederatedLearningYOLOv8/blob/master/src/federated_learning_yolov8.ipynb) to use federated learning.

Open [Google Colab](https://colab.research.google.com/).

A pop-up window will appear, asking to create a notebook or to load an existing one. You need to load it.

There are 2 ways to do it:
- Select the "Load" section in the top-right corner, and load the downloaded notebook.
- Or select the "Github" section, and paste the link of this repo. Colab will find the notebooks of this repo, and you can select the one needed.

Executing the cells will download all the datasets needed, otherwise you can upload your dataset wich must be in the right format needed by YOLOv8.

## Datasets

The original dataset contains 655 images, while 2 new datasets - containing 1000 and 1500 images respectively - have been created using augmentation techniques.

## Training

The training of the model was made both without and with federated learning. For the latter, 2 training methods were used: The first one where the 3 clients were chosen randomly, and the other one where the 3 clients with the best performance (based on mAP) were chosen.

## Built With

* [Colab](https://colab.research.google.com/) - Online platform by Google that allows writing and executing Python code directly in the browser, using cloud-based computing resources.
* [Roboflow](https://roboflow.com/) - Platform that facilitates the management, preparation, and annotation of datasets for training computer vision models.
* [YOLOv8](https://docs.ultralytics.com/) - The latest version of the acclaimed real-time object detection and image segmentation model.