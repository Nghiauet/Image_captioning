# Image Captioning with Resnet18 and Transformer Decoder
## Introduction
This project aims to implement an image captioning system using the Resnet18 for image embedding and Transformer Decoder for word embedding. The dataset used in this project is the uitviic_captions_train2017 dataset, which is a Vietnamese image captioning dataset.

## Requirements
Python 3.x
PyTorch
Transformers
Numpy
Pandas
## Dataset
The uitviic_captions_train2017 dataset consists of images and their corresponding captions in Vietnamese. The dataset can be downloaded from the official website of the UIT-VIIC image captioning challenge.

## Model Architecture
The model architecture consists of two main parts: the Resnet18 for image embedding and the Transformer Decoder for word embedding. The Resnet18 takes an image as input and outputs a fixed-length feature vector, which is then fed into the Transformer Decoder to generate the corresponding caption.

## Usage
To train the model, first download and extract the uitviic_captions_train2017 dataset. Then run `notebook.ipynb` (written for Google Colab), which trains the model and saves the checkpoints.

The evaluation cells at the end of `notebook.ipynb` generate captions for the test images and compute the scores below.

## Results
On the 231-image test split the model scored BLEU-1 0.71, BLEU-2 0.58, BLEU-3 0.47, BLEU-4 0.40, ROUGE-L 0.59 and CIDEr 1.13 (printed by the evaluation cell in `notebook.ipynb`; pycocoevalcap).



<img width="857" alt="image" src="https://user-images.githubusercontent.com/96003264/232093523-ea057895-793d-4772-a4a3-ac6368a63b1a.png">
<img width="983" alt="image" src="https://user-images.githubusercontent.com/96003264/232095363-48b4158c-d016-4278-b0b3-b5e4c3a03ae7.png">

<img width="928" alt="image" src="https://user-images.githubusercontent.com/96003264/232093322-4495c000-142a-47a2-a621-60f8208e9bc2.png">
