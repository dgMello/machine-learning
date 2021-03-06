# Machine Learning Engineer Nanodegree
## Capstone Proposal
Doug Mello
August 14th, 2019

## Proposal

### Domain Background

This project is derived from the computer vision field of research. This field is concerned with how computer programs process and analyze images. Convolutional neural networks (CNN), which are a class of deep neural networks have been applied to the computer vision field. CNN's can be used to solve problems in the computer vision field. See researched cited below on how CNN's have been used to solve computer vision problems.

- Face Recognition: A Convolutional Neural-Network Approach: http://www.cs.cmu.edu/afs/cs/user/bhiksha/WWW/courses/deeplearning/Fall.2016/pdfs/Lawrence_et_al.pdf

- MobileNets: Efficient Convolutional Neural Networks for Mobile Vision Applications: https://arxiv.org/pdf/1704.04861.pdf

On a personal level, I love dogs and this is a great way to learn about different breeds. I also word for a video security company, so anything I learn here may be able to used for our products.

### Problem Statement

A client wants to create an phone application that can do the following.

1. Take a picture of a dog or human.
2. Determine if the picture is of a human or dog.
4. If the picture is of a human it will output what type of dog breed the human looks like. If the picture is of a dog it will output what breed it is.

 We have been tasked with creating the algorithm that will identify the dogs and humans and provide the breed output. The algorithm should be able to take a image as an input and output a string that tells the user what the dog breed it is. This algorithm should work with as many dog breeds as possible, depending how many breeds the algorithm is trained on.

### Datasets and Inputs

The datasets in this project are images of dogs & humans and image labels with the dog name corresponding to each image. Each image will be jpeg & 256 x 256 pixels. Each dog image will be named after the dog breed the image is of. The dog images will be used to train the algorithm that will be used in the application. Human images will only be used for testing the algorithm. Images will also be used as inputs for the application itself. In a real world scenario an image dataset that could be use is the Stanford Dogs Dataset, http://vision.stanford.edu/aditya86/ImageNetDogs/. For the Dog Breed Classifier notebook, the datasets will be provided by Udacity.

The input dataset of image labels will be a csv file. Each label will the dog breed name. The labels will be created using an algorithm to take the name of each image and have the ".jpg" removed from it. This dataset will only be used to create the algorithm for the application. Once the application is in production it will no longer use labels as an input.

### Solution Statement

The solution to this problem will be to create an algorithm using the OpenCV library to detect humans and deep learning to detect dog breeds. The dog breed dataset images and labels will be fed into our algorithm to learn how to identify dog breeds. Separate images will be used to test the accuracy of the algorithm. Once a certain accuracies are reached the algorithm will be complete.

### Benchmark Model

There does not appear to be any benchmark models that have been created for this problem. However I will create a benchmark model our own results. Our algorithm should have an accuracy of at least 60%. Since our algorithm only has to perform one function to solve this problem the accuracy is the only benchmark to solve the problem.

For training our algorithm we can create a benchmark model for training loss and accuracy. During training of our algorithm our loss should be at most 0.600 and training accuracy should be at least 60%.

### Evaluation Metrics

For any type of algorithm where we are training a algorithm, we set a side a percent of the dataset to test our algorithm with. After we have trained our algorithm we will pass test images as input into our algorithm to test it. I will also use images found randomly on the internet to test as well. This will allow us to test our algorithm on data that was not on our dataset. With both tests of different images we should have an accuracy of 60%.

For training loss and accuracy our algorithm will have text output that will say what the current raining loss and accuracy is.

### Project Design
_(approx. 1 page)_

In this final section, summarize a theoretical workflow for approaching a solution given the problem. Provide thorough discussion for what strategies you may consider employing, what analysis of the data might be required before being used, or which algorithms will be considered for your implementation. The workflow and discussion that you provide should align with the qualities of the previous sections. Additionally, you are encouraged to include small visualizations, pseudocode, or diagrams to aid in describing the project design, but it is not required. The discussion should clearly outline your intended workflow of the capstone project.

1. Preprocess data. Separate data into training, testing & validation.
 - In this step we are going to take our dataset and break it into 3 separate datasets. The training set will be used for training our model. The testing set will be use to test our model after it's completed testing. The validation set will be use to check the accuracy of our model while it is training.

 - I will use the PyTorch DataLoader class to do this. This class separate the data for us as well shuffle & transform it. Doing this will help keep our data randomized so theirs less bias in our training.

2. Create the architecture of our model.

- In this step the architecture of our model will be designed.

3. Choose the loss function and optimizer for our model.

4. Train and validate the model.

 - In this step the model will be trained. All that is required is to run the code below. After this outputs of the current loss and accuracy will be displayed. This way I can see how the training is going.

model_transfer.load_state_dict(torch.load('model_transfer.pt'))

5. Test the model And Verify Accuracy Is At Least 60%.

- In this step we will input our test data into our newly trained model. If we have get at least 60% accuracy we know that the model will work for production. If the accuracy is below 60% steps 2-5 will need to be performed again until we achieve at least 60% accuracy.

-----------

**Before submitting your proposal, ask yourself. . .**

- Does the proposal you have written follow a well-organized structure similar to that of the project template?
- Is each section (particularly **Solution Statement** and **Project Design**) written in a clear, concise and specific fashion? Are there any ambiguous terms or phrases that need clarification?
- Would the intended audience of your project be able to understand your proposal?
- Have you properly proofread your proposal to assure there are minimal grammatical and spelling mistakes?
- Are all the resources used for this project correctly cited and referenced?
