
# Getting-Started

Resource for students getting started in Data Analytics/Data Science

![logo](https://github.com/ChapmanDAA/Getting-Started/blob/main/Logo/Full_Logo.jpeg?raw=true)

Welcome to the Chapman Data Analytics Association Github repository about all things Data Analytics/Data Science related. If you're asking, "I don't know anything about machine learning and it sounds cool but I don't know where to get started!", then you have come to the right place. This will act as a extensive guide to learning about the field of Data Science/Data Analytics, no matter your skill level.

---

# Table of Contents
- [Getting-Started](#getting-started)
- [Table of Contents](#table-of-contents)
- [Introduction](#introduction)
  - [What is Data Science/Data Analytics?](#what-is-data-sciencedata-analytics)
  - [How This Guide is Structured](#how-this-guide-is-structured)
  - [In Regards to Coding](#in-regards-to-coding)
    - [Python Resources](#python-resources)
    - [R Resources](#r-resources)
- [Topics in Machine Learning](#topics-in-machine-learning)
  - [Tools We Will Use](#tools-we-will-use)
    - [Python](#python)
    - [Jupyter Notebooks](#jupyter-notebooks)
      - [What is Jupyter Notebook?](#what-is-jupyter-notebook)
      - [Setting up Jupyter Notebook](#setting-up-jupyter-notebook)
        - [Downloading JupyterLab](#downloading-jupyterlab)
        - [Downloading Jupyter Notebook](#downloading-jupyter-notebook)
  - [Supervised Learning](#supervised-learning)
      - [Linear Regression](#linear-regression)
      - [Logistic Regression](#logistic-regression)
  - [Unsupervised Learning](#unsupervised-learning)
    - [Clustering](#clustering)
      - [K-Means](#k-means)
      - [DBSCAN](#dbscan)
      - [Hierarchical Cluster Analysis (HCA)](#hierarchical-cluster-analysis-hca)
    - [Dimensionality Reduction](#dimensionality-reduction)
      - [Principal Component Analysis (PCA)](#principal-component-analysis-pca)
    - [Neural Networks](#neural-networks)
- [More topics in Machine Learning](#more-topics-in-machine-learning)
  - [Deep Learning](#deep-learning)
- [Ethics](#ethics)
- [Challenges in ML](#challenges-in-ml)

---

# Introduction

Here in this repository we will be showing you a roadmap of how to get from knowing nothing at all to understanding how deep learning machine learning models work and the state of the art machine learning algorithms. A lot of resources will be linked throughout this guide, since we cannot possibly answer all the questions you may have (and frankly other people have done a way better job at explaining). 

*As you go through this guide, we would like to encourage you to think of this guide as a journey not a destination. The goal is not to learn one particular topic like Deep Neural Networks but to have tools in your arsenal to make sense of the data you are given.*

Knowing linear regression can be more important knowing how to code a neural network from scratch in certain scenarios. Plus a having a fundation in simpler topics can help you get an intuition for more complex topics!

## What is Data Science/Data Analytics?

## How This Guide is Structured

Since Data Science is a field with very polar ends when it comes to the theory and real world application, this guide will have a blend of both, hopefully explaining what the big ideas are while explaining in practical terms and how to use it.

## In Regards to Coding

The dreaded question for students with non-CS backgrounds: "Will I need to learn how to code?" The answer is Yes and No. While you won't have to get familiar with all intricacies of a coding language, learning some coding is very useful and highly recommended. 

There are two main languages when it comes to Data Science work: R and Python. The difference is that R is a more statistical programming language and Python is a more general purpose scripting language. Both are just as easy to learn but **we would recommend learning Python as a beginner, because there are so many helpful resources out there and its very commonly used in all parts of machine learning.** Most Universities also teach python as a first coding language to new CS students. If you attend Chapman, you can take the course CPSC 230 to learn Python.

Unfortunately, we won't be able to cover this topic as it is way outside the scope of this guide, but we will point you to some great resources on learning these languages. 

### Python Resources

- [CPSC230 Playlist](https://youtube.com/playlist?list=PLmxpwhh4FDm460ztGwXmIUcGmfNzf4NMW)
  - This is our recommended guide on learning python.
  - This is a video playlist from one of our Chapman professors, Dr. Chelsea Pelleriti, that explains not only how to get started with Python but also explains other programming topics.
  - This is our most recommended guide because it shows you how to set up vscode which we will be using as our default code editor when not using jupyter notebooks.
- [Learn Python Programming - Python Course](https://youtu.be/f79MRyMsjrQ)
  - This is a great suppliment to the previous playlist we thought we would include.
- [Python in 100 Seconds](https://youtu.be/x7X9w_GIm1s)
  -  This is a quick and concise video on what Python is, but it can be a lot of gibberish because they use a lot of programming jargon. It gives a high level idea of what Python is.
-  [Reddit Resource Links](https://www.reddit.com/r/learnpython/wiki/index/#wiki_new_to_programming.3F)
   -  This is a great text guide to learning Python and includes a lot of book recommendations if you learn better by reading.
-  [Python3 Documentation](https://docs.python.org/3/)
   -  An invaluable resource for writing Python code used by all Python developers. It contains all the information about Python3.

While we can't teach you how to use python, we will show you how to set up your coding environment and what libraries to install in the following sections.

### R Resources


---


# Topics in Machine Learning

## Tools We Will Use

- Python
- Python Libraries
  - [Scikit-Learn](https://scikit-learn.org/stable/index.html)
  - [Numpy](https://numpy.org/)
  - [Pandas](https://pandas.pydata.org/)
- [Jupiter Notebook](https://jupyter.org/) or [VSCode Jupiter Notebook extension](https://code.visualstudio.com/docs/datascience/jupyter-notebooks) or [Google Colab](https://colab.research.google.com/)

### Python

There are two major versions of Python: 2 and 3. We will be using Python 3 for everything, because Python 2 is depricated. Download Python [Here](https://www.python.org/downloads/). Click the big yellow button that says "Download Python 3.10.\*". Follow the instructions to install it and click the checkmark if it asks you if you want to ADD TO PATH.

### Jupyter Notebooks

#### What is Jupyter Notebook?

Jupyter Notebook is a web interface that you can run code, show its outputs and display plain text within a single page. Unlike regular text editors or IDEs, Jupyter Notebooks allow you to run python code by sections or lines instead of all at once making prototyping easier or displaying chunks of code more readable. Although it is a web interface, meaning it uses your web browser, it is run from your computer where you have to have Jupyter Notebook installed. 

This is **NOT** true for Google Colab, which runs from the cloud and doesn't need an installation. It's recommended that you use Google Colab if you have a low spec computer or don't want to go through the installation process, but note that on faster computers Colab will be significantly slower than running Jupyter Notebook from your machine because it needs to fetch the data from Google's servers. Other than the lack of installation, the interface should be very similar to Jupyter Notebooks and the same code should be able to run on both platforms without a problem. If you are using Google Colab, skip the next section.

#### Setting up Jupyter Notebook

There are a couple ways to set up Jupyter Notebooks. Jupyter Notebook is a standalone program that talks to the python interpreter to run code. JupyterLab is a more extensive development environment that is similar to an IDE. It has basically the same interface to Jupyter Notebook and runs the same but with some extra capabilities, like the ability to have multiple notebooks side by side on one screen. We would recommend getting JupyterLab because the interface is the same as Jupyter notebook with the same learning curve just with some extra quality of life features. Downloading Jupyter Notebook should not change anything though.

Make sure for any installation method, that you have Python3 already installed. To check type ```python3 --v``` into your terminal.

##### Downloading JupyterLab

1. Open up your terminal(Command Prompt/Windows Powershell)
2. ```pip install jupyterlab```
3. You should be able to launch JupyterLab with ```jupyter-lab```

##### Downloading Jupyter Notebook

1. Open up your terminal(Command Prompt/Windows Powershell)
2. ```pip install notebook```
3. You should be able to launch JupyterLab with ```jupyter notebook```

Official Installation Guide [Here](https://jupyter.org/install)

## Supervised Learning

#### Linear Regression

#### Logistic Regression

## Unsupervised Learning

### Clustering

#### K-Means

#### DBSCAN

#### Hierarchical Cluster Analysis (HCA)

### Dimensionality Reduction

#### Principal Component Analysis (PCA)

### Neural Networks



# More topics in Machine Learning

## Deep Learning

# Ethics

# Challenges in ML

