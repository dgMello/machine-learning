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

The datasets in this project are images of dogs and image labels with the dog name corresponding to each image. Each image will be jpeg & 256x256 pixels. Each image will be named after the dog breed the image is of. The images will be used to train the algorithm that will be used in the application. Images will also be used as inputs for the application itself. The image dataset is from the Stanford Dogs Dataset, http://vision.stanford.edu/aditya86/ImageNetDogs/.

The input dataset of image labels will be a csv file. Each label will the dog breed name. The labels will be created using an algorithm to take the name of each image and have the ".jpg" removed from it.

### Solution Statement
_(approx. 1 paragraph)_

In this section, clearly describe a solution to the problem. The solution should be applicable to the project domain and appropriate for the dataset(s) or input(s) given. Additionally, describe the solution thoroughly such that it is clear that the solution is quantifiable (the solution can be expressed in mathematical or logical terms) , measurable (the solution can be measured by some metric and clearly observed), and replicable (the solution can be reproduced and occurs more than once).

### Benchmark Model
_(approximately 1-2 paragraphs)_

In this section, provide the details for a benchmark model or result that relates to the domain, problem statement, and intended solution. Ideally, the benchmark model or result contextualizes existing methods or known information in the domain and problem given, which could then be objectively compared to the solution. Describe how the benchmark model or result is measurable (can be measured by some metric and clearly observed) with thorough detail.

### Evaluation Metrics
_(approx. 1-2 paragraphs)_

In this section, propose at least one evaluation metric that can be used to quantify the performance of both the benchmark model and the solution model. The evaluation metric(s) you propose should be appropriate given the context of the data, the problem statement, and the intended solution. Describe how the evaluation metric(s) are derived and provide an example of their mathematical representations (if applicable). Complex evaluation metrics should be clearly defined and quantifiable (can be expressed in mathematical or logical terms).

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
