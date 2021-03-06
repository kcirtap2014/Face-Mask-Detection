<h1 align="center">Face Mask Detection</h1>

in contribution to [Face Mask Detection](https://github.com/chandrikadeb7/Face-Mask-Detection) in an open source contest [Student Code-in](https://scodein.tech/)

<div align= "center">
  <h4>Face Mask Detection system built with OpenCV, Keras/TensorFlow using Deep Learning and Computer Vision concepts in order to detect face masks in static images as well as in real-time video streams.</h4>
</div>

## Motivation

In the present scenario due to Covid-19, there is no efficient face mask detection applications which are now in high demand for transportation means, densely populated areas, residential districts, large-scale manufacturers and other enterprises to ensure safety. Also, the absence of large datasets of **‘with_mask’** images has made this task more cumbersome and challenging.

## Tech/framework used

- [OpenCV](https://opencv.org/)
- [Caffe-based face detector](https://caffe.berkeleyvision.org/)
- [Keras](https://keras.io/)
- [TensorFlow](https://www.tensorflow.org/)
- [MobileNetV2](https://arxiv.org/abs/1801.04381)

## Features

Our face mask detector didn't use any morphed masked images dataset. The model is accurate, and since we used the MobileNetV2 architecture, it’s also computationally efficient and thus making it easier to deploy the model to embedded systems (Raspberry Pi, Google Coral, etc.).

This system can therefore be used in real-time applications which require face-mask detection for safety purposes due to the outbreak of Covid-19. This project can be integrated with embedded systems for application in airports, railway stations, offices, schools, and public places to ensure that public safety guidelines are followed.

## :file_folder: Dataset

The dataset used can be downloaded here - [Click to Download](https://drive.google.com/drive/folders/1XDte2DL2Mf_hw4NsmGst7QtYoU7sMBVG?usp=sharing)

This dataset consists of **3835 images** belonging to two classes:

- **with_mask: 1916 images**
- **without_mask: 1919 images**

The images used were real images of faces wearing masks. The images were collected from the following sources:

- **Bing Search API** ([See Python script](https://github.com/chandrikadeb7/Face-Mask-Detection/blob/master/search.py))
- **Kaggle datasets**
- **RMFD dataset** ([See here](https://github.com/X-zhangyang/Real-World-Masked-Face-Dataset))

## :key: Prerequisites

All the dependencies and required libraries are included in the file <code>requirements.txt</code> [See here](https://github.com/chandrikadeb7/Face-Mask-Detection/blob/master/requirements.txt)

## 🚀&nbsp; Installation

1. Clone the repo

```
$ git clone https://github.com/chandrikadeb7/Face-Mask-Detection.git
```

2. Change your directory to the cloned repo and create a Python virtual environment named 'test'

```
$ mkvirtualenv test
```

3. Now, run the following command in your Terminal/Command Prompt to install the libraries required

```
$ pip3 install -r requirements.txt
```

## :bulb: Working

1. Open terminal. Go into the cloned project directory folder and type the following command:

```
$ python3 train_mask_detector.py --dataset dataset
```

2. To detect face masks in an image type the following command:

```
$ python3 detect_mask_image.py --image images/pic1.jpeg
```

3. To detect face masks in real-time video streams by activating the camera type the following command

```
$ python3 detect_mask_video.py
```

or to load a video

```
$ python3 detect_mask_video.py --video <video_file>
```

## :key: Results

#### Our model gave 93% accuracy for Face Mask Detection after training via <code>tensorflow-gpu==2.0.0</code>

![](https://github.com/chandrikadeb7/Face-Mask-Detection/blob/master/Readme_images/Screenshot%202020-06-01%20at%209.48.27%20PM.png)

#### We got the following accuracy/loss training curve plot

![](https://github.com/chandrikadeb7/Face-Mask-Detection/blob/master/plot.png)

## Streamlit app

Face Mask Detector webapp using Tensorflow & Streamlit

command

```
$ streamlit run app.py
```

## Images

<p align="center">
  <img src="Readme_images/1.PNG">
</p>
<p align="center">Upload Images</p>

<p align="center">
  <img src="Readme_images/2.PNG">
</p>
<p align="center">Results</p>

## :+1: Credits

- [Chandrika Deb](https://github.com/chandrikadeb7)
- [https://www.pyimagesearch.com/](https://www.pyimagesearch.com/)
- [https://www.tensorflow.org/tutorials/images/transfer_learning](https://www.tensorflow.org/tutorials/images/transfer_learning)
