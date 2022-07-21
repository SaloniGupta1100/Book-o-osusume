# Book-o-osusume

![Python](https://img.shields.io/badge/Python-3.8-blueviolet)
![Framework](https://img.shields.io/badge/Framework-Flask-red)
![Frontend](https://img.shields.io/badge/Frontend-HTML/CSS/JS-green)


It aims to recommends books on the basis of popularity and give personalized recommendation on the basis of user's previous reads using various machine learning algorithms.

A recommendation engine is a class of machine learning which offers relevant suggestions to the customer.  Before the recommendation system, the major tendency to buy was to take a suggestion from friends. But Now Google knows what news you will read, Youtube knows what type of videos you will watch based on your search history, watch history, or purchase history.

A recommendation system helps an organization to create loyal customers and build trust by them desired products and services for which they came on your site. The recommendation system today are so powerful that they can handle the new customer too who has visited the site for the first time. They recommend the products which are currently trending or highly rated and they can also recommend the products which bring maximum profit to the company. 

In a very general way, recommender systems are algorithms aimed at suggesting relevant items to users (items being movies to watch, text to read, products to buy, or anything else depending on industries).


*Watch Demo* : <a href="https://youtu.be/4PPGD_YRQnU">Video Demo</a>

*Live* : <a href="https://book-o-osusume.herokuapp.com/">Try the Web App</a>

## Table Of Contents

[Installation](#installation)

[Tech Stack](#tech-stack)

[Data Description](#data-description)

[Similarity Score](#similarity-score)

[How Cosine Similarity works](#how-cosine-similarity-works)

[Support and Contact](#support-and-contact)


## Installation

To use this Project Follow the steps below:-

1. Clone the Repo

```bash

    git clone https://github.com/SaloniGupta1100/Book-o-osusume
```

2. Install the requirements

```bash
  
   pip install -r requirements.txt
```


3. Open your terminal/command prompt from your project directory and run the file  ``` main.py``` by executing the command  ``` python main.py```


4. Start Client : Go to your browser and type the address in the address bar.

```bash
  http://127.0.0.1:5000/ 
```

## Tech Stack

In spite of all the smart devices that exist today in the world, one thing that is common is - web and internet browsers. I selected my application to be a web application so that a large number of users are able to use it with ease and connect together

*FrontEnd:* HTML, CSS, VanilaJs

*BackEnd:* flask

*PythonLibraries:* numpy, pandas, jinja2, pickle

## Data Description
The Book-Crossing dataset comprises 3 files. 
<a href="https://www.kaggle.com/datasets/arashnic/book-recommendation-dataset?resource=download">Click to view the data set used </a>

### 1. Users
Contains the users. Note that user IDs ( ) have been anonymized and map to integers. Demographic data is provided ( , Age) if available. Otherwise, these fields contain NULL values.

### 2. Books
Books are identified by their respective ISBN. Invalid ISBNs have already been removed from the dataset. Moreover, some content-based information is given (Book-Title, Book-Author, Year-Of-Publication, Publisher), obtained from Amazon Web Services. Note that in the case of several authors, only the first is provided. URLs linking to cover images are also given, appearing in three different flavors (Image-URL-S, Image-URL-M, Image-URL-L), i.e., small, medium, large. These URLs point to the Amazon website.

### 3. Ratings
Contains the book rating information. Ratings (Book-Rating) are either explicit, expressed on a scale from 1-10 (higher values denoting higher appreciation), or implicit, expressed by 0.

#
We tried to make models from various perspective like
### 1. POPULARITY BASED MODEL
#### 1.1 Highest total book rating
Books are arranged in such a way that the books with the highest sum total of ratings are at the top.

#### 1.2 Most number of times rated
Books are arranged in such a way that books that have been rated the most number of times irrespective of the rating are at the top.


### 2. MEMORY BASED COLLABORATIVE FILTERING - ITEM BASED
Find similar items based on pearson correlation and took weighted average of ratings.

### 3. MODEL BASED COLLABORATIVE FILTERING 1
We used Scikit Surprise library for this model based approach.
Surprise is an open-source Python library that makes it easy for developers to build recommender systems with explicit rating data.


## Similarity Score 

   How does it decide which item is most similar to the item user likes? Here come the similarity scores.
   
   It is a numerical value ranges between zero to one which helps to determine how much two items are similar to each other on a scale of zero to one. This similarity score is obtained measuring the similarity between the text details of both of the items. So, similarity score is the measure of similarity between given text details of two items. This can be done by cosine-similarity.
   
## How Cosine Similarity works
  Cosine similarity is a metric used to measure how similar the documents are irrespective of their size. Mathematically, it measures the cosine of the angle between two vectors projected in a multi-dimensional space. The cosine similarity is advantageous because even if the two similar documents are far apart by the Euclidean distance (due to the size of the document), chances are they may still be oriented closer together. The smaller the angle, higher the cosine similarity.
  
  ![image](https://user-images.githubusercontent.com/36665975/70401457-a7530680-1a55-11ea-9158-97d4e8515ca4.png)

  
More about Cosine Similarity : [Understanding the Math behind Cosine Similarity](https://www.machinelearningplus.com/nlp/cosine-similarity/)



## Support and Contact

Email: officialetc01@gmail.com
