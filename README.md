# Table of Contents

1. [Installation](#installation)
2. [Project Motivation](#motivation)
3. [File Descriptions](#files)
4. [Modelling](#model)
5. [Performace](#performance)
6. [Results](#results)
7. [Licensing, Authors, and Acknowledgements](#licensing)

# Installation <a name="installation"></a>

There should be no necessary libraries to run the code here beyond the Anaconda distribution of Python. The code should run with no issues using Python versions 2.*.

# Project Motivation <a name="motivation"></a>
For this project, I was motivated to use SF Crime Dataset taken from SF OpenData to answer the following questions

* What are most common type of crimes that happen in SF?
* Do these crimes get resolved?
* Is there a trend in time when a particular type of crime is common?
* What types of crimes are common for a particular day?
* Any seasonality trend in the crimes?

# File Descriptions <a name="files"></a>
There is 1 notebooks available here to showcase work related to the above questions. This notebook is exploratory in searching through the data pertaining to the questions showcased by the notebook title. Markdown cells were used to assist in walking through the thought process for individual steps.

This notebook also contains the code to model the question to predict if the case can be resolved or not based on the features created.

# Modelling <a name="model"></a>

Now let's try to build a simple model based on the data we have to see if a given crime will be resolved or not. Let's use following features that we already have

* Category
* PdDistrict
* is_resolved (Predicting column)
* DayOfWeek
* part_of_day

# Performance <a name="performance"></a>
We trained a simple Logistic Regression and tried to predict if a given case can be resolved or not and obtained an average F1 score of 81.4% with average Precision and Recall of 81.4% and 81.6% respectively.

# Results <a name="results"></a>

The main findings can be found on the blog post [here](https://medium.com/@pradeep.thalasta/san-francisco-crime-analysis-b887ebad83ab)


# Licensing, Authors, Acknowledgements <a name="licensing"></a>
Must give credit to SF OpenData for the data. You can find the Licensing for the data and other descriptive information at the Kaggle link available [here](https://www.kaggle.com/c/sf-crime). Otherwise, feel free to use the code here as you would like!

