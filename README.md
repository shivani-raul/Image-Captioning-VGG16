# Image-Captioning-VGG16
The project repo “Image Captioning” is about defining and training a CNN and RNN Networks in order to automatically generate captions for an Image. Hence we created a Machine learning model to generate captions for images. This project uses VGG16, a CNN model for feature extraction. These features are converted to image captions by RNN. Flickr 8K dataset is used for training of this model.
# Dataset
The dataset used is flickr8k. You can request the data here. An email for the links of the data to be downloaded will be mailed to your id. Extract the images in Flickr8K_Data and the text data in Flickr8K_Text.
# Requirements
Tensorflow
Keras
Numpy
Pandas
Pillow
# Flow Design of The project
1. Data collection
2. Data Preprocessing — Text
3. Data Preprocessing — Images
4. Training
5. Testing
6. Model Architecture
7. Evaluation
# Learnings
1. How a convolutional neural network and LSTM can be combined to generate captions
to an image.
2. How to utilize the beam search algorithm to consider multiple captions and select the
most probable sentence.
# References
Orchid Engg, (Jan 2018). Image Captioning using Deep Neural Architectures.
[online]arXiv.org.Available at: https://arxiv.org/abs/1801.05568

Harshall Lamba, Data Science , s. (2018). Teaching Computers to describe pictures , Image
Captioning with Keras.[online]towardsdatascience.org. Available at: https://towardsdatascience.com/image-captioning-with-keras-teaching-computersto-describe-pictures-c88a46a311b8

Faizan, Analytics Vidya (2018).Automatic Image Captioning using Deep Learning (CNN
and LSTM).[online]analyticsvidya.com. Available at:
https://www.analyticsvidhya.com/blog/2018/04/solving-an-image-captioning-taskusing-deep-learning/

# Output
The output of the model is a caption to the image.

# Results
Following are a few results obtained after training the model for 70 epochs.

Image	Caption
	Generated Caption: A brown dog is running in the water.
	Generated Caption: A tennis player hitting the ball.
	Generated Caption: A child in a helmet is riding a bike.
	Generated Caption: A group of people are walking on a busy street.
On providing an ambiguous image for example a hamsters face morphed on a lion the model got confused but since the data is a bit biased towards dogs hence it captions it as a dog and the reddish pink nose of the hamster is identified as red ball

Image	Caption
	Generated Caption: A black dog is running through the snow with a red ball.
In some cases the classifier got confused and on blurring an image it produced bizzare results

Image	Caption
	Generated Caption: A brown dog and a brown dog are playing with a ball in the snow.
	Generated Caption: A little girl in a white shirt is running on the grass.
