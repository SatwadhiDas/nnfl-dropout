In this research project, we will focus on the effects of changing dropout rates on the MNIST dataset. Our goal is to reproduce the figure below with the data used in the research paper. The purpose of this project is to learn how the machine learning figure was produced. Specifically, learning about the affects to classification error when changing/not changing the dropout probability.

# How to reproduce analysis:
- Must have python 2.7.X installed
- Best to run in a UNIX/Linux Environment

# Software/Libraries used
We used Google Colab to run dropout on the MNIST dataset, Matplotlib to assist in recreating the figure in the paper.  Numpy was imported to get the plotting to have the same step size on the x and y-axis.

## Purpose of Coding Project:
Exploring the effects of varying values of the tunable hyperparameter 'p' (the probability of retaining a unit in the network) and the number of hidden layers, 'n', that affect error rates. When the product of p and n is fixed, we can see that the magnitude of error for small values of p has reduced (fig. 9a) compared to keeping the number of hidden layers constant (fig. 9b).

## Problem Setting:
With limited training data, many complicated relationships between inputs/outputs will be a result of sampling noise. They will exist in the training set, but not in real test data even if it is drawn from the same distribution. This complication leads to overfitting, this is one of the algorithms to help prevent it from occurring. The input for this figure is a dataset of handwritten digits, and the output after adding dropout are different values that describe the outcome of applying the dropout method. All in all, less error is outcome after adding dropout.

## Data Sources:
A real world problem that this can apply to is google searching, someone may be searching for a movie title but they might only be looking for images because they are more visual learners. So dropping out the textual parts, or brief explanations will help you focus on the image features. The article states where they retrieve the data from (http://yann.lecun.com/exdb/mnist/). Each image is a 28x28 digit representation. The y labels seem to be the image data columns.

