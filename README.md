# Book-o-osusume
It aims to recommends books on the basis of popularity and give personalized recommendation on the basis of user's previous reads using various machine learning algorithms.

A recommendation engine is a class of machine learning which offers relevant suggestions to the customer.  Before the recommendation system, the major tendency to buy was to take a suggestion from friends. But Now Google knows what news you will read, Youtube knows what type of videos you will watch based on your search history, watch history, or purchase history.

A recommendation system helps an organization to create loyal customers and build trust by them desired products and services for which they came on your site. The recommendation system today are so powerful that they can handle the new customer too who has visited the site for the first time. They recommend the products which are currently trending or highly rated and they can also recommend the products which bring maximum profit to the company. 

In a very general way, recommender systems are algorithms aimed at suggesting relevant items to users (items being movies to watch, text to read, products to buy, or anything else depending on industries).


*Watch Demo* : <a href="https://drive.google.com/file/d/19QrszJ03D6Qcg6gijL74d1WQ54JF382J/view?usp=sharing">Video Demo</a>

*Live* : <a href="https://book-o-osusume.herokuapp.com/">Try the Web App</a>

## Table Of Contents
[Data Description](#Data-Description)

[Installation / Getting Started](#installation)

[Tech Stack](#tech-stack)

[Future Scope](#future-scope)

[Bug Log](#bug-log)

[Support & Contact](#support-&-contact)

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


## Installation

To use this Project Follow the steps below:-

1. Clone the Repo

```bash

    git clone https://github.com/SaloniGupta1100/Book-o-osusume
```

2. install NPM Packages

```bash
  
   npm install i
```


3. Do the required for activating .env files


4. Start Client

```bash
   
   npm start
```


## Tech Stack

In spite of all the smart devices that exist today in the world, one thing that is common is - web and internet browsers. I selected my application to be a web application so that a large number of users are able to use it with ease and connect together

*Client:* HTML, CSS

*Server:* flask, numpy, pandas, jinja2, pickle

## Future Scope

-Adding more information the places for more efficient planning of the trip.

-Adding wishlist feature and list of places done exploring.

-Forming community Section where like-minded people and share their reviews and planout next trip with a group those have same level of energy.

-Adding hybrid recommendation system in the homepage.


## Bug Log

-Sometimes Google Maps API shows error and doesn't work. 

-Budget of the places is set to default.

## Support and Contact

Email: saloniofficial.09@gmail.com
