# Generate TV Scripts Deep Learning :tv:

you can find the project's files at this link: https://github.com/udacity/deep-learning-v2-pytorch/tree/master/project-tv-script-generation

# Project Overview:
This project for the Deep Learning Nanodegree program of Udacity,It's RNN project, In this project I generated my own Seinfeld TV scripts using RNNs. I used part of the Seinfeld dataset of scripts from 9 seasons. The Neural Network that I built is generate a new "fake" TV script, based on patterns it recognizes in this training data.

# Project Instructions:
## Instructions
1. Clone the repository and navigate to the downloaded folder.
```
git clone https://github.com/iSarah-alsh/Generate-TV-Scripts-.git
cd Generate-TV-Scripts

```
2. Open `the dlnd_tv_script_generation.ipynb` file. Of course, you can find HTML version of the file.
```
jupyter notebook dlnd_tv_script_generation.ipynb
```
3. Read and follow the instructions! This repository already includes the dataset in a form of txt flie in data folder.

 # Project Information:
 ## Contents
 - Get the Data
- Explore the Data
- Implement Pre-processing Functions
     - Lookup Table
     - Tokenize Punctuation
- Pre-process all the data and save it
- Check Access to GPU
- Input
     - Batching
     - Test your dataloader
     - Sizes
     - Values
- Build the Neural Network
     - Define forward and backpropagation
- Neural Network Training
     - Train Loop
     - Hyperparameters
     - Train
- Generate TV Script
     - Generate text
     - Generate a new script

## Main RNN model:
RNN is very good for sequential data like Text because each input depends on previous one RNN also has a memory which captures information about what has been calculated so far so, it's able to looking back for a few steps. RNN perform the same task for every element of sequence.
In this project I used LSTM (Long-Short Term Memory) which is much better at capturing long-term.

## RNN Architecture:

![0_LyfY3Mow9eCYlj7o](https://user-images.githubusercontent.com/46428156/61139741-a16eee80-a4d2-11e9-8058-83bc9626f52b.png)

Image Resource: https://codeburst.io/generating-text-using-an-lstm-network-no-libraries-2dff88a3968

# Dataset:
I used part of the Seinfeld dataset of scripts from 9 seasons.
https://www.kaggle.com/thec03u5/seinfeld-chronicles#scripts.csv

# Libraries:
The list below represents main libraries and its objects for the project.

- PyTorch ([LSTM](https://colah.github.io/posts/2015-08-Understanding-LSTMs/))
