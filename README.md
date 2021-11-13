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







