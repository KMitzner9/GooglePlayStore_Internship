# GooglePlayStore_LiveProject
Files for the Google Play Store Live Project
This project is a part of the [Tech Academy Data Science Bootcamp](https://www.learncodinganywhere.com/).

#### -- Project Status: [Completed]

## Project Introduction
The purpose of this project is to address client requests regarding information from the Google Play Store data set. The client is an app developer that wanted information on popular and well-reviewed apps in order to decide which kinds of apps to create.  Based on their request, I produced statistical analysis, visualiztions and machine learning models for this data set.

### Partner
* [Prosper IT Consulting](https://www.learncodinganywhere.com/ProsperITConsulting)

### Methods Used
* Descriptive Statistics
* Machine Learning
* Data Visualization

### Technologies
* Python
* Pandas, jupyter
* Jupyter Notebook
* matplotlib, seaborn

## Project Description
I worked with a spreadsheet from the Google Play Store that contained over 10,000 records and 13 columns. I answered a variety of questions based on client request to help them direct their app development team. Here are the requested tasks from the client:
* Client would like to know the mean price and mean number of installs for Health and Fitness.
* Client would like to see how many entertainment apps have a content rating of mature.
* Client would like a Jupyter Dashboard.
* Client would like to see which apps are similar by Rating.

## Project Details

In the following sections, I will give a brief summary of each clients request and how I provided my solution. For a more detailed exploration of each request, including code examples, please reference the Report linked in that section

## Client would like to know the mean price and mean number of installs for Health and Fitness

For this task, I isolated only the apps in the health and fitness category. After examining some summary statistics, it was clear the set contained many outliers. Due to the sheer amount of free apps, every paid app was considered an outlier, so I decided to split the data into paid and free apps and perform my analysis on each group. I used interquartile range to determine which outliers to remove, and then generated the requested summary statistics for each category. Based on the information gathered, I advised the client that free apps are much more likely to be popular, and also gave them an estimate of how many installs they might expect for a paid app.

For more information view the [full report](https://github.com/KMitzner9/GooglePlayStore_LiveProject/blob/main/reports/User_Story_98.docx) and [Jupyter Notebook](https://github.com/KMitzner9/GooglePlayStore_LiveProject/blob/main/98_Final.ipynb).


## Client would like to see how many entertainment apps have a content rating of mature

This was the simplest and most straightforward of the client requests. I used the groupby() method to isolate the entertainment category, organize it by content rating, and count each app in that category. I was able to give the client an exact number of apps, but also used a bar graph and pie chart to show what proportion of the apps belonged to this category as well.

For more information view the [full report](https://github.com/KMitzner9/GooglePlayStore_LiveProject/blob/main/reports/User_Story_100.docx) and [Jupyter Notebook](https://github.com/KMitzner9/GooglePlayStore_LiveProject/blob/main/100_scratch.ipynb).

## Client would like a Jupyter Dashboard

For this assignment, I was asked to create an interactive dashboard using Jupyter Dashboards, which would allow the client to select any category of apps and see the number of apps that belong to that category, the mean rating of apps in that category, and the total number of installations. Unfortunately the functionality of Jupyter Dashboards is, well, non-functional. In the spirit of done being better than perfect, I created an interactive widget in the Jupyter notebook that the client could use that had the same functionality, if not the clean appearance, of a traditional dashboard. I offered to create a Shiny app instead, but due to the time constraints, the client declined.

For more information, please view the [full report](https://github.com/KMitzner9/GooglePlayStore_LiveProject/blob/main/reports/User_Story_95.docx) and [Jupyter Notebook](https://github.com/KMitzner9/GooglePlayStore_LiveProject/blob/main/GPS_95_Dashboard.ipynb).

## Client would like to see which apps are similar by Rating

Specifically, the client requested a clustering algorithm to see which apps are similar by Rating and Category. I created a data frame containing only the app names, categories, and ratings to be saved for my analysis, and I created another dataframe with only the features to be used by the machine learning algorithms. Based on my data I decided to use KMeans, DBSCAN, and MeanShift methods to determine the clusters. I performed some hyperparameter tuning to find the best models and appended the model-based cluster labels to the data set containing app names. I was then able to use aggregate functions to determine which apps were clustered together. Unfortunately, due to the small set of features, the apps were clustered based on the predetermined categories assigned. In the future I would use more than just two features for the models. 

This assigment was a learning process for me and I discuss what I learned and how I might do things differently in the [full report](https://github.com/KMitzner9/GooglePlayStore_LiveProject/blob/main/reports/User_Story_99.docx).
View my [Jupyter Notebook](https://github.com/KMitzner9/GooglePlayStore_LiveProject/blob/main/99_scratch.ipynb) to see how I created my models.
[CSV](https://github.com/KMitzner9/GooglePlayStore_LiveProject/blob/main/GPS_clusters.csv) containing the cluster labels from each model

## Discussion/Conclusion

Working on a live data set was challenging, fun, and a great opportunity for growth! I took on some simpler projects to demonstrate the skills I am confident in, and took on some more challenging tasks in order to learn and grow as a Data Scientist. I developed my own workflow routines and became very comfortable using pandas to manipulate and clean the data. I had to work under a timeline and produce results based on client needs rather than my own curiosity, so I had to be stringent with my time management and keep in constant communication with my project manager. I encountered several tasks that required me to research and learn on the job, and have a much better understanding of what my strengths are how I can improve them with self-study. I was able to provide useful insights for my client while simultaneously improving my Python and general Data skills.

## Contact
* Send me an email at KMitzner9@gmail.com 
* Contact me via my portfolio site [portfolio site](http://www.kenziemitzner.com/)
* Connect with me on [LinkedIn](https://www.linkedin.com/in/kenzie-mitzner/)
