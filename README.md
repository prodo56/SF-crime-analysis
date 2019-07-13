# Data Exploration

Let us try to answer the following questions

* What are most common type of crimes that happen in SF?
* Do these crimes get resolved?
* Is there a trend in time when a particular type of crime is common?
* What types of crimes are common for a particular day?
* Any seasonality trend in the crimes?


# Conclusions
So to summarize we went through the SF Crime dataset obtained from Kaggle (https://www.kaggle.com/c/sf-crime/data) and did some data exploration to see what the data tells us. Here is what we found

* `LARCENY/THEFT` and `OTHER OFFENSES` happen to be the top 2 crimes reported in SF
* Major number of crimes are reported at the Southern District and Southern District happen to have resolved a vast % of cases they received.
* Out of all the cases reported more than 60% of the cases don't get resolved and from the categories of crimes reported `LARCENY/THEFT` has a very low probability of getting resolved. Also, what was interesting to see from the plot is that major % of cases reported under `DRUG/NARCOTIC` get resolved. Ofcourse, no country wants drug infestation, so they have high priority.
* Crimes are consistent throught the week. What was interesting to see was that `LARCENY/THEFT` has higher chances during Fridays and Saturdays. 
* High number of `LARCENY/THEFT` happen mostly during the afternoons and have higher rates at dusk, evening and at night times!!

# Modeling

Now let's try to build a simple model based on the data we have to see if a given crime will be resolved or not. Let's use following features that we already have

* Category
* PdDistrict
* is_resolved (Predicting column)
* DayOfWeek
* part_of_day

# Results
We trained a simple Logistic Regression and tried to predict if a given case can be resolved or not and obtained an average F1 score of 81.4% with average Precision and Recall of 81.4% and 81.6% respectively.
