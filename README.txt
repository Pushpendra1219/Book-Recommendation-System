Welcome to Book Recommender system 

Objective

The main goal is to develop a mechanism for users to receive book recommendations. In some businesses, recommender systems are crucial because, when used well, they can generate significant revenue or serve as a means of differentiating oneself from rivals.

Methods Used

Descriptive Statistics Data Visualization Machine Learning

Technologies

Python Pandas Numpy Matplotlib Seaborn Scikit-learn Surprise Flask

Data

The Book-Crossing dataset comprises 3 files.

Users : Contains the users. Note that user IDs (User-ID) have been anonymized and map to integers. Demographic data is provided (Location, Age) if available. Otherwise, these fields contain NULL values.

Books : Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (Book-Title, Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web Services. Note that in the case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavors (Image-URL-S, Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the Amazon website.

Ratings : Contains the book rating information. Ratings (Book-Rating) are either explicit, expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit, expressed by 0.

Project Description

EDA - Performed exploratory data analysis on numerical and categorical data.

Data Cleaning - Missing value imputation,Outlier Treaatment

Feature Selection - Used User-ID,ISBN and Books-Rating for model development.

Model development - Tried Popularity based model and Collaborative filtering (Both Memory based and Model based).

Flask API = It is used for building web applications. The back-end is developed in Flask which exposes prediction endpoints to predict using a trained classifier and send the result back to the front-end for easy consumption.


Getting Started

Clone this repo (for help see this tutorial).

First create a virtual environment in pyhton using 
virtualenv -p python3 .

Then activate the environment using 
soruce bin/activate

Install the required python dependencies using 
pip install -r requirements.txt

Start Flask using 
FLASK_APP=app.py flask run


Raw Data

Users data is being kept here within this folder in raw_data.

Ratings data is being kept here within this folder in raw_data..

Books data is being kept here withing folder in raw_data.

Complete notebook containing Data exploration/Data processing/transformation/model development is being kept here.
