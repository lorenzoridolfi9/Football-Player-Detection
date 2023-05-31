# Football-Player-Detection ⚽️ 👀 

## This repository contains project files of Computer Vision. In particular, Yolov8 have been applied for object detection tasks, which can create model that recognize football players and others in the frame.

## Dataset 📊 

### Soccer Players Detection Image is the name of the dataset used in the following project, containing frames of soccer games. it is divided into three parts:
- __Train-set(80%)__: 531 training frames of the model
- __Validation-set(10%)__: 66 frames of model validation
- __Test-set(10%)__: 66 frames for testing the model

The dataset was taken from Roboflow, which also annotated the classes for each frame. You can see the Roboflow universe from [this link](https://universe.roboflow.com/).

If you want, you can download this dataset from [this link](https://drive.google.com/drive/folders/1s9HUL9wM5MFtSfPqBl86zFfpE_Hkxd_U?usp=sharing) in my Google Drive.


## Process of Analysis ⚙️

the code is a google colab notebook that has simplified model training using Nvidia Tesla T4 GPUs.
there are 4 classes present:
- football players
- goalkeeper
- referee
- ball

Training was done for 50 epochs, although after various tests it is possible to confirm that a number of epochs of 20 is sufficient for satisfactory results.

## Results 📈
At the end of training, good results are achieved in both the training-set and validation-set, reaching a total __mAP__ of __0.87__ and __0.85__, respectively.
the most hostile class to detect remains ball with a mAP of __0.50__ in both the training and validation sets.
The other classes are predicted correctly, with a mAP reaching a value of __0.99__ in both datasets.

## Video test 🎞️
Finally, the model was tested in an .mp4 video capturing part of a soccer match between two teams.
