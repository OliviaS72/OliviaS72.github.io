# Olivia Schultheis
## Data Science Portfolio
### Python, R, and Tableau

### PROJECT 1: Python
### Convolutional Neural Network to Classify Rock, Paper, Scissors Images from Tensorflow Dataset
Link: [Rock, Paper, Scissors Convolutional Neural Network](https://github.com/OliviaS72/RockPaperScissors_CNN)

**This project used the 'rock_paper_scissors' dataset from tensorflow_datasets. There are 2,520 images in the training dataset and 372 images in the testing dataset. All of these images show hand gestures of either rock, paper, or scissors. The layers for the Convolutional Neural Network are shown below:**

<img src= /assets/img/CNN_layers_rockpaperscissors.png width="400" height="400">

**The overall testing accuracy of this model was about 77%.**

**While the details of the composition of the neural network could be technically discussed (which is provided in detail within the wiki of the above GitHub link) one of the most important details to explore with this project is to consider how the classification could be further improved. Below are 25 misclassified images. The classification associated with "p: " is the predicted class for each image below it, while the classification associated with "e: " is the expected, or actual, class for each image below it. Class 0 is for rock, 1 is for paper, and 2 is for scissors.**

<img src= /assets/img/testing_misclass_preview.png width = "600" height = "600" >

**More images were used for training than for testing, but within the 2,520 training images, an equal amount (840) of each class were present and within the 372 testing images, an equal amount (124) were present. The preview of 25 misclassified images is a part of a group of 86 total misclassifed images out of 372.**

**Out of the misclassified images, 25 were rock, 4 were paper, and 57 were scissors. The model seems to be doing the best at predicting paper, but struggles to distinguish between rock and scissors. The model could likely be improved if more pictures were included in training that clearly were different among the rock and scissors photos.**

### Project 2: R
### Plot of Daily Closing Stock Price for Amazon and Target in January 2024. 
## Data is from Nasdaq website##
## Target: https://www.nasdaq.com/market-activity/stocks/tgt
## Amazon: https://www.nasdaq.com/market-activity/stocks/amzn

Github Repo with actual CSV files used (only plotted data for January 2024) : [Amazon Target Line Plot](https://github.com/OliviaS72/AmazonTargetStock)

RPubs Publication of Code with Visualization: [Rpubs Amazon Target Line Plot](https://rpubs.com/Olivias3/1206691)

Visualization: 






