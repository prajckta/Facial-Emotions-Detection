This project is an implementation of a Face Emotion Detection system using OpenCV and PyTorch. The system is designed to detect facial expressions and predict emotions from images. It utilizes a pre-trained deep learning model trained on a dataset of labeled facial expressions. The dataset can be downloaded from The kaggle dataset. The dataset can be downloaded from https://www.kaggle.com/datasets/ananthu017/emotion-detection-fer/data.

Dataset Description
Dataset contain 35,685 examples of 48x48 pixel gray scale images of faces divided into train and test dataset. Images are categorized based on the emotion shown in the facial expressions (happiness, neutral, sadness, anger, surprise, disgust, fear).

Model
We have used a custom model including CNN ,max pooling and linear layers. The model architecture can be found in file main.py. Also added normalization and dropout layers to reduce overfitting.
Train accuracy: 85.06170382165605% Validation accuracy=61.76709624985487% there is still a lot of scope to reduce overfitting.
Usage
haarcascade_frontalface_default.xml is used to detect exact faces in the image, this is directly used from https://github.com/opencv/opencv/tree/4.x/data/haarcascades.

Funtion predict_with_labels predicts the emotion present in the image, it takes image and the cascade to detect faces as input arguments.

Further Scope :
Adjusting the size of label in the input image around the box(no optimal values for font-size and thickness).
More number faces detection than that present in the input image.
#Some examples showing working of face detection algorithm on real dataset.




![Screenshot 2024-08-03 090207](https://github.com/user-attachments/assets/8eea8c76-bd0b-4ca5-9a58-30b894774c1d)
