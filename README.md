# Image-Captioning
The Image captioning model has been implemented using the Sequential API of keras. It consists of three components:

An encoder CNN model: A pre-trained CNN is used to encode an image to its features. In this implementation ResNet50 model is used as encoder and with its pretrained weights loaded. The last softmax layer of ResNet50 is removed and the vector of dimention (2048,) is obtained from the second last layer.

A word embedding model: Pre-trained glove embeddings have been used in this project which outputs a word embeddings of shape (1848,50).

A decoder RNN model: A LSTM network has been employed for the task of generating captions. It takes the image vector and partial captions at the current timestep and input and generated the next most probable word as output.

Steps for image captioning:-

1)Data collection
        
2)Understanding the data

3)Data Cleaning

4)Loading the training set

5)Data Preprocessing — Images

6)Data Preprocessing — Captions

7)Data Preparation using Generator Function

8)Word Embeddings

9)Model Architecture

10)Inference
