# Machine Learning Engineer Nanodegree
## Capstone Proposal
Doug Mello
August 14th, 2019

## Proposal
_(approx. 2-3 pages)_

### Domain Background

This project is derived from the computer vision field of research. This field is concerned with how computer programs process and analyze images. Convolutional neural networks (CNN), which are a class of deep neural networks have been applied to the computer vision field. CNN's can be used to solve problems in the computer vision field. See researched cited below on how CNN's have been used to solve computer vision problems.

- Face Recognition: A Convolutional Neural-Network Approach: http://www.cs.cmu.edu/afs/cs/user/bhiksha/WWW/courses/deeplearning/Fall.2016/pdfs/Lawrence_et_al.pdf

- MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications: https://arxiv.org/pdf/1704.04861.pdf

On a personal level, I love dogs and this is a great way to learn about different breeds. I also word for a video security company, so anything I learn here may be able to used for our products.

### Problem Statement

A client wants to create an phone application that can take a picture of a dog and then display the type of breed the dog is. We have been tasked with creating the algorithm that will identify the dogs. The algorithm should be able to take a image as an input and output a string that tells the user what the dog breed is. This algorithm should work with as many dog breeds as possible, depending how many breeds the algorithm is trained on.

### Datasets and Inputs

The datasets in this project are images of dogs and image labels with the dog name corresponding to each image. Each image will be jpeg & 256x256 pixels. Each image will be named after the dog breed the image is of. The images will be used to train the algorithm that will be used in the application. Images will also be used as inputs for the application itself. In a real world scenario an image dataset that could be use is the Stanford Dogs Dataset, http://vision.stanford.edu/aditya86/ImageNetDogs/. For the Dog Breed Classifier notebook, the datasets will be provided by Udacity.

The input dataset of image labels will be a csv file. Each label will the dog breed name. The labels will be created using an algorithm to take the name of each image and have the ".jpg" removed from it. This dataset will only be used to create the algorithm for the application. Once the application is in production it will no longer use labels as an input.

### Solution Statement

The solution to this problem will be to create an algorithm using deep learning. The dog breed dataset images and labels will be fed into our model to learn how to identify dog breeds. Separate images will be used to test the accuracy of the model. Once a certain accuracy is reached the algorithm will be complete.

### Benchmark Model

There does not appear to be any benchmark models that have been created for this problem. However I will create a benchmark model our own results. Our model should have an accuracy of at least 60%. Since our algorithm only has to perform one function to solve this problem the accuracy is the only benchmark to solve the problem.

For training our model we can create a benchmark model for training loss and accuracy. During training of our model our loss should be at most 0.600 and training accuracy should be at least 60%. 

### Evaluation Metrics
_(approx. 1-2 paragraphs)_

In this section, propose at least one evaluation metric that can be used to quantify the performance of both the benchmark model and the solution model. The evaluation metric(s) you propose should be appropriate given the context of the data, the problem statement, and the intended solution. Describe how the evaluation metric(s) are derived and provide an example of their mathematical representations (if applicable). Complex evaluation metrics should be clearly defined and quantifiable (can be expressed in mathematical or logical terms).

For any type of algorithm where we are training a model, we set a side a percent of the dataset to test our algorithm with. After we have trained our model we will pass test images as input into our model to test it.

### Project Design
_(approx. 1 page)_

In this final section, summarize a theoretical workflow for approaching a solution given the problem. Provide thorough discussion for what strategies you may consider employing, what analysis of the data might be required before being used, or which algorithms will be considered for your implementation. The workflow and discussion that you provide should align with the qualities of the previous sections. Additionally, you are encouraged to include small visualizations, pseudocode, or diagrams to aid in describing the project design, but it is not required. The discussion should clearly outline your intended workflow of the capstone project.

-----------

**Before submitting your proposal, ask yourself. . .**

- Does the proposal you have written follow a well-organized structure similar to that of the project template?
- Is each section (particularly **Solution Statement** and **Project Design**) written in a clear, concise and specific fashion? Are there any ambiguous terms or phrases that need clarification?
- Would the intended audience of your project be able to understand your proposal?
- Have you properly proofread your proposal to assure there are minimal grammatical and spelling mistakes?
- Are all the resources used for this project correctly cited and referenced?
