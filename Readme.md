# Image Captcha Solver

As a part of coursework related to the subject 'Scalable Computing' in Trinity College Dublin, 
Project1 and Project2 targets to solve large amount of image captchas using convulation layer.

## Project 1: Solving the list of 5 image captchas
Steps performed-
1. Generated 100000 sample image captchas through generate.py by randomly generating the captchas out of the symbols (A-Z,0-9), depending on the inputs like width, height of captcha image, Length of captchas in characters, no. of captchas to generate, path to output folder, symbols file.
2. Split the data into train and validate in the 80/20 ratio.
3. Trained and tested the model using the generated captchas under train and validate data as input through train.py. Train code contains the training model using Keras neural network library that works on layers.
4. Conv2D(2D Convolution Layer) is used to create a convolution kernel that is wind with layers input which helps produce a tensor of outputs and scaling the input pixel values.
5. Trained model architecture is saved to .json file.
6. Now this .json file is used to classify the given 5 captchas using classify.py.

## Project 2: Solving the image captchas but this time a lot more!
Same steps were performed as in Project 1.
The only difference was this time generated 200000 captchas for training the model. 
Made use of Google Cloud instances to train the data on GPU.

## Files contained
1. generate.py - script to generate large amount of sample captchas through randomness
2. train.py -  script to train the model by inputting part of sample captchas that were generated
3. classify.py - Model trained is used to classify the new set of image captchas through this script
4. commands.txt - set of commands through with other scripts are executed defining batch size and epochs iterated for training and classification

###### Keywords
Image captcha, tensor flow, keras, consulation layer, scalable computing
