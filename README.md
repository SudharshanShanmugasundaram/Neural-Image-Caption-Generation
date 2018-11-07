# Neural-Image-Caption-Generation

Image caption generation is the problem of generating a descriptive sentence of an image. The fact that humans (e.g you) can do this with remarkable ease makes this a very interesting/challenging problem for AI, combining aspects of computer vision (in particular scene understanding) and natural language processing.

We load the VGG model in Keras using the VGG class. We will remove the last layer from the loaded model, as this is the model used to predict a classification for a photo. We are not interested in classifying images, but we are interested in the internal representation of the photo right before a classification is made. These are the “features” that the model has extracted from the photo.Then we feed these extracted features along with the words generated at each iteration to a LSTM network which generates captions.

# Dataset
The dataset is available for free. You must complete a request form and the links to the dataset will be emailed to you.

You can use the link below to request the dataset:

[Dataset Request Form](https://forms.illinois.edu/sec/1713398)

Within a short time, you will receive an email that contains links to two files:

Flickr8k_Dataset.zip (1 Gigabyte) An archive of all photographs.
Flickr8k_text.zip (2.2 Megabytes) An archive of all text descriptions for photographs.
Download the datasets and unzip them into your current working directory. You will have two directories:

Flicker8k_Dataset: Contains 8092 photographs in JPEG format.
Flickr8k_text: Contains a number of files containing different sources of descriptions for the photographs.
The dataset has a pre-defined training dataset (6,000 images), development dataset (1,000 images), and test dataset (1,000 images).

# Requirements
1. Python
2. Tensorflow
3. Keras
4. NLTK
5. Pickle

*I would recommend atleast 8 Gigs of RAM when you run it on your local machine.* 

*If you have GPU make use of the Progressive Model which is included.*
