# Multi Class Text Classification #

**Software Product Classification and Categorization
(With Product Description and License Information)**

**Intro:**

* Software product business is evolving very fast 
* Internet has grown rapidly and businesses now are going digital 
* Software products account for substantial economic activity all over the world
* It has now become a compulsion to have access to the latest data on every subject 
* Purchases of Software licenses has been increasing from large enterprises to individual users
* This project focuses on Machine learning classification models for software categorization

---------------------------------------------------------------------------------------------------

**Requirements & Tools**

Supervised learning uses a training set to train the model, the training set should have inputs and correct labelled outputs.
The Bigger and Quality Data will produce a better Classification Model.
Web Scraping is used for Data Harvesting in current project.
Python 3.9.2  & Jupyter Notebook from Anaconda, Inc. is used as the IDE.

---------------------------------------------------------------------------------------------------

**Background**

- Software Asset Management is a business strategy that involves managing & optimizing assets.
- Aids in reclaiming budget and maximizing savings by controlling procurement and deployment of software licenses 

---------------------------------------------------------------------------------------------------

**Objectives**

* Understand the current scenario of software product classification and broad categories in which they could be placed.
* Designing a model that could correctly tag a particular software based on either keyword(s) in product name and from product description text.
* A search mechanism to extract the correct information from the web about a particular software. 
* To identify the product type (Licensable / Not-Licensable) of the software given that the License information is available in internet.

---------------------------------------------------------------------------------------------------

**Scope of Work**

Scope of this dissertation is to design and build a classification model using Machine Learning algorithms that could predict the software product category from software product description.
Retrieve license information for a given product if license data is available on public websites or e-Commerce / re-seller websites. 
Application areas: 
- Classification Model: To Categorize a software product.
- Information Extraction: To extract the correct information of a particular software.

---------------------------------------------------------------------------------------------------

**Product Categories**

United Nations Standard Product and Service Code (UNSPSC) is taken as reference for understanding product categories. UNSPSC is a classification framework for all products and services. UNSPSC is such a classification structure which is:
- Open Standard - publicly available
- Not proprietary
- Available to all to read and implement
- No royalty or license fees for usage

---------------------------------------------------------------------------------------------------

**Software Categories**
Security
Development Software
Business Software
Internet Software
Networking Software
Browsers
Communications
Video
Desktop Software
Photography
Utilities
Gaming Software

---------------------------------------------------------------------------------------------------

**Supervised Machine Learning**

Supervised learning as the name suggests is the model learning method/algorithm inspired and trained under supervision.
It is defined by the use of pre-labelled datasets to train algorithms that would then be applied on an unknown/new data to predict un-labelled outcomes accurately.
Supervised learning uses a training set to train the model.
Supervised learning are of two types : Classification and Regression
Classification refers to predictive modelling algorithm(s) where a class label is predicted for a given set of input data.
Regression algorithm will attempt to establish a relation between dependent variable and independent variable(s) such that the variable values are predicted based on independent variables.

---------------------------------------------------------------------------------------------------

### Web Scraping ###

Web scraping is the automated gathering of data from the Internet. Python Libraries for Web scraping:
Pandas : Pandas is a library that has functions and methods for data-analysis and data-manipulation in Python. 
Beautiful Soup : Beautiful Soup is a python library for harvesting data from HTML and XML files. 
requests.get( ) is the requests library method for making HTTP requests in Python.
Data Source : We need to harvest thousands for data samples that should contain the following:
Software Product name
Software Products Description
Product Category
Licensing information (if available)

---------------------------------------------------------------------------------------------------

### HTML Inspection ###

Right click on the web-page and choosing “Inspect” will open a window to see HTML code behind the web-page.
It also enables a highlighter as we hover over various parts of the Web-page so as to know which parts of HTML code is responsible for displaying what components of the web-page.

HyperText Markup Language (HTML) is a standard language for creating Webpages:
It describes the structure and layout of the Webpage
It consists of a series of elements
It dictates the web browser on how to organize and display the content on webpages
It has specific sections such has headings, paragraphs, links, frames to organize the content and the order

Tags and Attributes are the main components of HTML 

---------------------------------------------------------------------------------------------------

### Python Requests ###

Python Requests is a library used to enable the HTTP requests easily in the python code.
‘pip’ command could used to install Pandas, BeautifulSoup and request to the Path directory in windows Command prompt or Mac/Ubuntu Terminal.
requests.get( ): GET method indicates trail to get or retrieve data from specified source 
The .content attribute of the requests object gives us the raw bytes of the response payload which could be converted into a string using the character encoding via the .text attribute 
The usual response code for a successful connection to the specified URL is 200. The response code for unsuccessful connection is 404 which means the specified URL is Not Found.

---------------------------------------------------------------------------------------------------


### BeautifulSoup HTML parser ###

The BeautifulSoup (‘doc.html’, ‘html.parser’) would go to the HTML document and parse thought the content of HTML code.
The useful information that needs to be captured from the HTML code could be found by identifying the HTML classes and HTML tags in which the information that is embedded. 

---------------------------------------------------------------------------------------------------

### Extracting Information from HTML Classes and HTML Tags ###

*Information to be captured such as Products name & Product description
*These attributes could be extracted from div tags and HTML classes
*The find_all( ) method in BeautifulSoup finds all instances where the given tags & classes are found 
*Throughout the web API, we could filter based on tags & classes on the attributes and extract the text
*The process could be repeated to extract all the relevant information required

---------------------------------------------------------------------------------------------------

### Pandas DataFrame ###

A DataFrame is a 2-dimensional data structure with rows and columns, it could be thought of as a spreadsheet or SQL table.
The information collected via Web Scraping can be loaded to a xlsx file or csv file with DataFrame.
DataFrame is one of the functionality of Pandas library
DataFrame features:
Columns headers are usually of different data types and represent attributes of dataset.
DataFrame are mutable, i.e.; could be expanded with additional information or remove existing data.
DataFrame is labelled with respect to rows and columns.
DataFrame could be created from various inputs: Lists or Dictionaries

---------------------------------------------------------------------------------------------------

### Python Dictionaries ###

Dictionaries could be easily converted to DataFrame which then could be loaded to a csv file for later use.
Dictionaries in Python are usually a set of data having a relationship of Key : Value pairing. Each Key is separated from its value by a colon. The whole data in the dictionary is enclosed in curly braces { }.
Dictionary construction using Product, Description, Platform, Price as column headers or Keys of the dictionary, the information collected via web scraping are stored as values against the column headers.
The dictionary data could be converted into a DataFrame by using the DataFrame method in the pandas library.

---------------------------------------------------------------------------------------------------


### Classification ###

Classification algorithm tries to accurately assign the test data to specific category or categories.
Classification refers to predictive modelling algorithm or technique where a class label is predicted for a given set of input data.
Classification will require training dataset with lots of inputs and precise outputs from which it would learn.
Classification algorithms are evaluated based on their output(s) i.e., predictions.
Prediction accuracy is a popular metric to discern the performance of the Classification model.
Prediction accuracy is never perfect, but a model having an accuracy of 80%-90% is an considered an good model.

---------------------------------------------------------------------------------------------------

### Classification types and algorithms ###

Three main types of classifications:
Binary Classification (contains two class labels – positive/negative or True/False)
Multi-Class Classification (multiple class labels with only one predicted label per input)
Multi-Label Classification (multiple class labels with more than one prediction label per input)
Few of the widely used algorithms for Classification are:
Decision Trees 
Support Vector Machines 
K-Nearest Neighbours

---------------------------------------------------------------------------------------------------


### Multi-Class Classification ###

Multi-Class Classification refers
to classification tasks that have more than 2 class labels.

Data is classified among a range of known classes.

The number of class labels will depend on the Classification task and dataset that is to be classified.

Predicting a sequence of words, Text translation, Face recognition are few examples of Multi-Class Classification.

The size of the vocabulary would define the number of features.
The text from which the predictions are made could be tens or hundreds of thousands of words in size depending upon on the task.

---------------------------------------------------------------------------------------------------

### Multi Class Text Classification ###

Text classification is a supervised learning method which will need labelled data to train the model.
It requires Data Analysis & Text Processing techniques on data before applying to a training model.
Features are attributes from which the prediction behaviour is based on, we could create features from the text descriptions.
Scikit-learn is a Python library to create a matrix of features from count of the words in the text descriptions, few methods in Scikit-learn to accomplish this:
CountVectorizer
Term frequency-inverse document frequency (tfidf)

---------------------------------------------------------------------------------------------------

### Data Visualization ###

Matplotlib is a python library to create interactive visualizations in Python.
It provides an object-oriented API for embedding plots into applications.
matplotlib.pyplot is a collection of command style functions for data visualisations.
Few of the widely used visualisations:
Bar (Make a bar plot)
Hist (Plot a histogram)
Pie (Plot a pie chart)

---------------------------------------------------------------------------------------------------

### Features Extraction ###

Scikit learn has several methods with which features could be extracted from a dataset.
TfidfVectorizer and similarly CountVectorizer imported from Scikit learn follow 4 sequential steps:

Import the function
Instantiate the method by assigning it to a variable
The Fit( ) method is used to fit the data according to the parameters passed
Transform( ) is used to transform the fitted data into a matrix or a vectored matrix

---------------------------------------------------------------------------------------------------

### train_test_split ###

train_test_split : will split the arrays or matrices into random train and test data subsets.
train_test_split( ) function takes in a parameter a labelled data as input and splits the dataset into two subsets for training and  testing. 
We don't have to divide the dataset manually.
Single call for splitting data in a one liner into training subset and testing subset.
Takes in as parameters the data array that needs to be divided.

---------------------------------------------------------------------------------------------------

### CountVectorizer and TfidfTransformer ###

CountVectorizer converts a group of text descriptions to a matrix of token counts.
It has the capability to tokenize a collection of text and build a vocabulary of common words. (Bag of Words)
TfidfTransformer will transforms a count matrix (Bag of words) to a normalized tf or tfidf representation.
The goal of using tfidf is to scale down the impact of tokens that occur very frequently in a given dataset and hence avoid the features that are empirically less informative than features that occur in a small fraction in the training dataset.

Term Frequencies – denotes number of occurrences of each word in a text description divided by the total number of words in that description.
Term Frequency - Inverse Document Frequency – (tfidf) downscales the weights for those words that occur in many documents or almost all documents and are therefore less informative and redundant than those that occur only in a smaller portion.

---------------------------------------------------------------------------------------------------

### Model Selection ###

Support Vector Classification’s (sklearn.svm.SVC) implementation is based on libsvm which is one of the fit( ) method available in Scikit learn for developing a model.
Any classifier algorithm imported from Scikit learn follow 4 sequential steps:

For larger datasets LinearSVC is more practical method.
Another model available in Scikit learn is Naive Bayes classifier : sklearn.naive_bayes.MultinomialNB

---------------------------------------------------------------------------------------------------


### LinearSVC ###

The objective of a LinearSVC (Support Vector Classifier) is to fit to the data provided, such that  the  "best fit" model would divide and categorize the data.
Linear Support Vector Classifier (SVC) method generally tries to construct a linear kernel function to perform classification and it would usually perform well if the input dataset has large number of samples.
The features needed to be passed in to LinearSVC ( ) to evaluate what the "predicted" class is.
After fitting the model on training data, predictions could be made and model accuracy score can be calculated.

---------------------------------------------------------------------------------------------------


### Improving the Prediction accuracy scores ###

Predictions in Classification problems, especially text classification would require Good Data.

The Quality of the labelled data directly corresponds to the better prediction scores.

There are few techniques that could be implemented to improve prediction accuracy:

-Add more data
-Feature Engineering & Feature Selection	
-Testing Multiple algorithms
-Treat missing and Outlier values

---------------------------------------------------------------------------------------------------


### Conclusions ###

The major scope of the project involves in analysing a group of text descriptions, loading the file content with the corresponding categories, using feature extraction techniques to create feature vectors that would be suitable for developing machine learning classification models to perform categorization.
Web Scraping methods are implemented to extract the data required to train the Classifier.
Web harvesting methods and technologies are increasing in relevance as data has become the basis on which all decision-making processes are implemented.
Software Product Classification find major applications in Software Asset Management (SAM), which is rapidly becoming an Billion dollar industry.

---------------------------------------------------------------------------------------------------

-------------------------------*********************************-----------------------------------

---------------------------------------------------------------------------------------------------












