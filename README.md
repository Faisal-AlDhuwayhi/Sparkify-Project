# Sparkify Project
Sparkify is an imaginary, popular digital music service similar to Spotify or Pandora. Menus of users stream their favorite songs to your service every day either using the free tier or using the premium subscription model. Every time a user interacts with the service, it generates data. All this data contains the key insights for
keeping your users happy and helping your business thrive.
**It's the job to predict which users are at risk to churn** either downgrading from premium to free tier or cancelling their service altogether.

So in this project, we will manipulate large and realistic datasets with Spark to engineer relevant features for predicting churn. We will use Spark MLlib to build machine learning models with large datasets, far beyond what could be done with non-distributed technologies like scikit-learn.

## Project Motivation
Predicting churn rates is a challenging and common problem that data scientists and analysts regularly encounter in any customer-facing business. If you can accurately identify these customers before they leave, your business can offer them discounts and incentives,
potentially saving your business millions in revenue. Additionally, the ability to efficiently manipulate large datasets with Spark is one of the highest-demand skills in the field of data. 

## Project Components
The project consists of several components:
1. **Loading and Cleaning Dataset**
2. **Exploratory Data Analysis**
3. **Feature Engineering**
4. **Modeling**

## Instructions
This project requires Python 3.x version. And in order to complete this project, you need to install the following libraries:
- [pyspark](http://spark.apache.org/docs/latest/api/python/)
- [numpy](https://numpy.org/)
- [pandas](https://pandas.pydata.org/)
- [matplotlib](https://matplotlib.org/)
- [seaborn](https://seaborn.pydata.org/)
  
You will also need to have software installed to run and execute an [iPython Notebook](http://ipython.org/notebook.html).

## Data 
This project has utilized mini subset (128MB) of the full dataset available (12GB). Optionally, you can choose to deploy a Spark cluster on the cloud using [AWS](https://aws.amazon.com/) or [IBM Cloud](https://www.ibm.com/sa-en/cloud) to analyze a larger amount of data. Currently we have the full 12GB dataset available to you if you use AWS. If you use IBM, you can download a medium sized dataset to upload to your cluster. However, the project is prepared to be used in large settings.

**Full Sparkify Dataset:** s3n://udacity-dsnd/sparkify/sparkify_event_data.json

**Mini Sparkify Dataset:** s3n://udacity-dsnd/sparkify mini_sparkify_event_data.json

**Medium Sparkify Dataset:** https://video.udacity-data.com/topher/2018/December/5c1d6681_medium-sparkify-event-data/medium-sparkify-event-data.json


## Results
After comparing the F1-Score for each model and applying cross-validation, it has been pointed that the **Gradient boosted tree** model performed best for predicting customer churn.

Furthermore, there are more features that could be generated to represent the characteristics of the user. There is room for improvement on applying sophisticated hyperparameter tuning to the model for resulting in better outcomes. Also, the process of feeding the input to the model could be pipelined to adapt to the big data settings.

## Additional
The project results are based mainly on a mini subset of the data (128MB), so it is recommended to finish the project with the full dataset (12GB). It would be beneficial and effective to observe the results with the full dataset and see the differences.

**My blog post about the project can be found [here on Medium website](https://medium.com/@alduohy11/predicting-customer-churn-using-apache-spark-3672470f8fe1).**