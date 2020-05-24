# Capstone Spark Project - Sparkify

### Overview 

Many music streaming provides (e.g. Spotify) collect huge amounts of data by collecting how users interact with their services (e.g. at which time a user is listen to a certain song etc.). These data contain valuable information to improve the services of the streaming providers. But the amount of generated data quickly exceeds the memory capacities of most personal computers. To still have the possibility to analyze this data, tools like Spark are necessary. Spark processes data in a distributed manner and as a result, Spark can also analyze data which does not fit into the memory of a single machine. Therefore, we use Spark in this Project to analyze user event log data of a music streaming service. 

### Objective

We will use Spark to analyze the churning behavior of the users of Sparkify. We will attempt to predict the likelihood of a user cancelling their service by using different machine learning models. We will compare the accuracy of each given model and then pick the most accurate and run it on the full 12GB dataset on a spark cluster on Amazon Web Services.

### The Data

The data at our disposal is a very granular log of the activities on the service's interface. It contains demographic information, user selection, timestamps, and more. Some of the available features are:

* Artist
* Authorization
* FirstName
* Gender
* Lastname
* Song length
* Payment level
* Location
* page
* Song
* Timestamp

### Dependencies

* pyspark
* Numpy
* Pandas
* matplot

### File description

* Sparkify.ipynb - Jupyter notebook employing pyspark to perform exploratory data analysis, metric definition, feature engineering, modeling, and model evaluation on the Sparkify data set.

### Summary results

The LogisticRegression was the best performing model out the three we chose. With our 7 engineered features, we were able to obtain an F1 score of 0.71 on the 'small' dataset when we ran it on a local machine. 

### Improvements
Improvements to the above results could be possible by applying e.g. the following approaches:

•	Creating more number of features
•	Training on a larger dataset, by deploying on cloud (AWS, IBM cloud)
•	Try more models, e.g. Deep Learning models
•	Try to find an additional data source which could be helpful for the considered task
