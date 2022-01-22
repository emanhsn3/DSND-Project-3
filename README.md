# Recommendations-with-IBM
This repo contains the submission of DSND *Experiment Design and Recommendations* project (Tested on Ubuntu 16.04 LTS and Python 3.x)

## Getting Started
This is a recommendation engine using the data of articles on the IBM Watson Studio platform where we analyze the interactions 
that users have with articles on the IBM Watson Studio platform, and make recommendations to them about 
new articles we think they will like.

Table of Contents of the notebook:

1. Exploratory Data Analysis
2. Rank Based Recommendations
3. User-User Based Collaborative Filtering
4. Matrix Factorization

6. Extras & Concluding

## Prerequisites
In order to run this project locally on your machine, you should've the following

- [pip](https://bit.ly/2x4hZQu)
- [numpy](https://scipy.org/install.html)
- [pandas](https://pandas.pydata.org/docs/getting_started/index.html#getting-started)
- [matplotlib](https://matplotlib.org/users/installing.html)

## Installation
Let's start first with installing the required libraries:

<code>python -m pip install --user numpy pandas matplotlib</code>

For more installation options for Windows/Mac check the hyperlinks provided in the **previous** section.

### Running the installation tests

If all the libraries are installed correctly open terminal (ctrl + alt + t) or any Python editor of your choice, in case you used terminal type <code>python3</code>

then type in the following  code, it should get executed with no errors:
```python
import numpy
import pandas
import matplotlib
```
## Now you are ready to run the code on your local machine, follow these steps:

- Get the datasets from the [IBM Watson Studion platform](https://www.ibm.com/eg-en/cloud/watson-studio)
- Clone the repo using: <code>git clone https://github.com/AbdelrahmanAEmam/Recommendations-with-IBM.git</code>
- Set the directories locations to be compatible with your datasets location
- Go to the repo location cd path/to/repo
- Finally, open Recommendations_with_IBM.ipynb (for best practice use jupyter notebook)

## Note
This code is tested on dataset provided by [IBM Watson Studio](https://www.ibm.com/eg-en/cloud/watson-studio).
In order to deploy this code on your own dataset, your data should follow the format of the given datasets.


## How the code works
**1. Exploratory Data Analysis**

Exploring the data we have with for the project and get to find an answer to basic questions (How many users we have?
How many articles? ..etc.).

**2. Rank Based Recommendations**

Finding the most popular articles simply based on the most interactions, 
these are then the articles we might recommend to new users depending on the popularity of the article (Most read articles)
since we don't have information about the user yet.

**3. User-User Based Collaborative Filtering**

Building better recommendations for the users of IBM's platform, 
by finding the other users that are similar in terms of the items *(articles)* they have interacted with.
Now our recommendations would be more personal for the users.


**4. Matrix Factorization**

Using a machine learning approach to building recommendations. Using the user-item interactions,
we will be building out a matrix decomposition. Using this decomposition, so we will get an insight of
how well we can predict new articles.

## Acknowledgments
- [Udacity Data Science Nanodegree Program](https://www.udacity.com/course/data-scientist-nanodegree--nd025)
- [IBM Watson Studio Platform](https://www.ibm.com/eg-en/cloud/watson-studio)
