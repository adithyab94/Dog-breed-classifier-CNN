[//]: # (Image References)

[image1]: ./images/sample_dog_output.png "Sample Output"

# Dog breed classifier project

The aim of the project is to create an application that is able to identify a breed of dog if given a photo or image as input. The Steps and results of the project are discussed elaborately on the following blog post in [Medium](https://medium.com/@adithya.b94/dog-breed-classifier-using-convolutional-neural-networks-c40da89435b6)

## Project Overview

This project is centered around the practical implementation of a Convolutional Neural Networks (CNN) for classifying dog breeds. An example output of the complete classifier is shown here:

![Sample Output][image1]

The goal of this project is for students to apply what we have learned of CNNs, to explore and become comfortable with using Keras to build CNNs and to analyse our results and look for ways to improve our models.

## Getting Started

There is only one notebook in this repo: `dog_app.ipynb`

### View-only

If you simply want to view the solution, open up `dog_app.html` for a complete notebook with all cells executed.

### Follow along Instructions

Assuming that your local development environment is setup with Keras and Tensorflow,
If you wish to replicate this notebook on your own machine, follow these instructions.

1. Clone the repository and navigate to the downloaded folder

```bash
git clone https://github.com/adithyab94/Dog-breed-classifier-CNN.git
cd dog-project
```

2. Download the [dog dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip). Unzip the folder and remove the zip file (to save space).

```bash
curl -o dogImages.zip https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/dogImages.zip
unzip dogImages.zip && rm -rf dogImages.zip
```

3. Download the [human dataset](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip).  Unzip the folder and place it in the repo, at location `path/to/dog-project/lfw`.  If you are using a Windows machine, you are encouraged to use [7zip](http://www.7-zip.org/) to extract the folder.

```bash
curl -o lfw.zip https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/lfw.zip
unzip lfw.zip && rm -rf lfw.zip
```

4. If you want to execute the code, you will need to download all the bottleneck features provided by Udacity. You can download them by using the curl command as above on the following urls:

- [VGG-19](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogVGG19Data.npz)
- [ResNet-50](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogResnet50Data.npz)
- [Inception](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogInceptionV3Data.npz)
- [Xception](https://s3-us-west-1.amazonaws.com/udacity-aind/dog-project/DogXceptionData.npz)

## Running the notebook

Open up the notebook using jupyter:

```bash
jupyter notebook dog_app.ipynb
```

Run through the code cells, but note that most of the training procedures require a good GPU to complete in a reasonable time.
