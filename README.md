# Olivia Schultheis
## Data Science Portfolio
### Python, R, and Tableau

### PROJECT 1: Python
### Convolutional Neural Network to Classify Rock, Paper, Scissors Images from Tensorflow Dataset
Github Repository Link: [Rock, Paper, Scissors Convolutional Neural Network](https://github.com/OliviaS72/RockPaperScissors_CNN)

**This project used the 'rock_paper_scissors' dataset from tensorflow_datasets. There are 2,520 images in the training dataset and 372 images in the testing dataset. All of these images show hand gestures of either rock, paper, or scissors. The layers for the Convolutional Neural Network are shown below:**

<img src= /assets/img/CNN_layers_rockpaperscissors.png width="400" height="400">

**The overall testing accuracy of this model was about 77%.**

**While the details of the composition of the neural network could be technically discussed (which is provided in detail within the wiki of the above GitHub link) one of the most important details to explore with this project is to consider how the classification could be further improved. Below are 25 misclassified images. The classification associated with "p: " is the predicted class for each image below it, while the classification associated with "e: " is the expected, or actual, class for each image below it. Class 0 is for rock, 1 is for paper, and 2 is for scissors.**

<img src= /assets/img/testing_misclass_preview.png width = "300" height = "400" >

**More images were used for training than for testing, but within the 2,520 training images, an equal amount (840) of each class were present and within the 372 testing images, an equal amount (124) were present. The preview of 25 misclassified images is a part of a group of 86 total misclassifed images out of 372.**

**Out of the misclassified images, 25 were rock, 4 were paper, and 57 were scissors. The model seems to be doing the best at predicting paper, but struggles to distinguish between rock and scissors. The model could likely be improved if more pictures were included in training that clearly were different among the rock and scissors photos.**

### Project 2: Python
### Recurrent Neural Network to Classify Text related to Science Fields of Chemistry, Biology, and Physics
Github Repository Link: [Science Comments Recurrent Neural Network](https://github.com/OliviaS72/RNNScienceText)

**This project uses a Kaggle dataset found here ([Kaggle Data for Science Comments](https://www.kaggle.com/datasets/vivmankar/physics-vs-chemistry-vs-biology/data)) to develop a recurrent neural network for text classification.**

**This dataset contains 10,281 comments relating to the fields of physics, chemistry, biology. The training dataset consists of 8,695 comments, and the testing data consists of 1,586 comments. The data is cleaned so that extra white space is replaced by blanks, urls, emojis, symbols, and pictographs are removed. Also, common stop words are removed and words are reduced to their roots, or stems. A tokenizer with GloVe Embedding is used to convert the text to numerical arrays that the neural network can actually use for training.**

**To alleviate the issue of short term memory with RNNs, which is when the information from words early on in the text does not have much impact by the time the network stops back propogation. In this project, I used a bidrectional LSTM (Long Short-Term Memory) layer which uses gates to have longer-term memory of past information.**

**The final accuracy of this model was 0.81. A plot of accuracy, loss, precision, and recall for the training and validation set is shown below:** <br> 

<img src = /assets/img/Metric_Plots_RNN_Science.png width = "600" height = "400">

**As can be seen in the above plots, overfitting does not seem to be an issue with this neural network because the training loss steadily decreases, and the validation loss never increases to a large degree. Also, the training accuracy steadily increases, and the validation accuracy never decreases to a large degree.**
