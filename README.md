# EDA_Project (Playstore Review Analysis)
### 📋 **Abstract**


 A few thousand new applications are uploaded to the Google Play Store on a regular basis. A large number of designers are working freely on designing the apps and making them successful. It is important for a developer to be aware of the correct path for designing a successful app. Since the majority of Play Store apps are free, it is quite difficult to understand how in-app purchases, in-app advertisements, and memberships contribute to an app's success. In this way, rather than focusing on the amount of revenue generated, an application's success is typically determined by the number of installations it has received and the customer reviews it has received over time. The goal of this experiment is to provide information that will help engineers better understand client wants and, in turn, aid in the product's widespread adoption. We have made an effort to understand the connections between many characteristics, such as whether an application is free or paid, what kind of user feedback it has, and how well it is rated.


### 💾 **Project Files Description**

This Project includes 1 colab notebook, 1 technical documentation as well as 1 presentation:

**Input Files:**

**Play Store Data.csv** - It contains the basic details of the app like number of user reviews, ratings, etc.
**User Reviews.csv** - It contains the user reviews and its sentiment score for the respective app.
Data Source:

**Dataset** - Dataset taken from Almabetter

**Output:**
**Google Colab** - All the outputs are visible in the provided colab notebook.

📖 **Introduction:**
In the current environment, it is clear that mobile apps play a significant part in every person's life. A designer needs to be aware of whether they are moving in the right direction or not in the face of immense challenges from all around the world. The application designers may need to find a way to maintain their current position in order to maintain this money and their position in the market. The dataset containing 10,000 apps is accessible to study the Android market. It can be looked at to analyse several categories, including family, communication, entertainment, tools, music, and cameras, among others. In this project, we look at the many data set characteristics that influence how well-liked an application is. We focused on answering questions like, "Which category has maximum number and minimum number of installation?" "Find out the most popular app" "How sentiment polarity affect in Rating?" The dataset has two CSV files for data analysis: Play Store Data User Reviews First, let's analyse the Play Store data. The Play Store data has 10841 rows and 13 columns.

**Dataset Information**

### **Play Store Data**

play store dataframe has 10841 rows and 13 columns. The 13 columns are identified as below:



*   **App** - It tells us about the name of the application.
*   **Category** - It gives the category to the app,like educational,sports,games etc.

*   **Rating** - It contains the average rating of the respective app received from its users.
*   **Reviews** - It shows us about the total number of users who have given a review for the application.

*   **Size** - It tells us about the size being occupied by the application on the mobile phone.

*  **Installs** - It tells us about the total number of installs/downloads for the application.
*   **Type** - It states whether an app is free to use or paid.

*  **Price** - It states the price payable to install the app. For free type apps, the price is zero.

*  **Content Rating** - It states whether or not an app is suitable for all age groups or not.

*   **Genres** - It tells us about the various other categories to which an application can belong.
*  **Last Updated** - It tells us about the when the application was updated.

*  **Current Ver** - It tells us about the current version of the application.

*  **Android Ver** - It tells us about the android version which can support the application on its platform.


### User Review dataset
user_reviews dataframe has 64295 rows and 5 columns. The 5 columns are identified as follows:

* **App:** Contains the name of the app with a short description (optional).
* **Translated_Review:** It contains the English translation of the review dropped by the user of the app.
* **Sentiment:** It gives the attitude/emotion of the writer. It can be ‘Positive’, ‘Negative’, or ‘Neutral’.
* **Sentiment_Polarity:** It gives the polarity of the review. Its range is [-1,1], where 1 means ‘Positive statement’ and -1 means a ‘Negative statement’.
* **Sentiment_Subjectivity:** This value gives how close a reviewers opinion is to the opinion of the general public. Its range is [0,1]. Higher the subjectivity, closer is the reviewers opinion to the opinion of the general public, and lower subjectivity indicates the review is more of a factual information.

### 📋 **Objectives**

Google Play Store is one of the top app markets in the world, and it is quite popular among millions of people. As the app store market is growing, the demand for developers is also growing. The Play Store allows users to install different kinds of apps as per their interests and have access to rate and comment on the apps as per their experiences, which is called a review.

To make a successful and engaging app, developers should have knowledge of the users choices and preferences for features like the app's size, price, Android version,when it was last updated, etc.

Before developing the apps, developers should also know the user sentiment of other apps that have similar features to the future app.

Two datasets are provided for the analysis of users choice and sentiment: one is basic information about the apps, and the other is about users reviews and sentiments about particular apps. Both datasets need to be examined in order to identify the important factors that influence app engagement and success.

### 📔 **What is Exploratory Data Analysis?**
Exploratory data analysis (EDA) is used by data scientists to analyse and investigate data sets for patterns and anomalies (outliers), form hypotheses based on our understanding of the dataset, and summarise their main characteristics, often employing data visualisation methods. It is an important step in any data analysis or data science project. It helps determine how best to manipulate data sources to get the answers you need.

EDA involves generating summary statistics for numerical data in the dataset and creating various graphical representations to understand the data better and make it more attractive and appealing.

The following are the various steps involved in the EDA process:

Problem Statement: We shall brainstorm and understand the given data set. We shall study the attributes present in it and try to do a philosophical analysis about their meaning and importance for this problem.

Hypothesis: Upon studying the attributes present in the database, we shall develop some basic hypotheses on which we can work and play with the data to look for the varied results that we can get out of it.

Univariate Analysis: This is the simplest form of analysing the data. In this, we would initially pick up a single attribute and study it in and out. It doesn't deal with any sort of co-relation, and its major purpose is to describe. It takes data, summarises that data, and finds patterns in the data.

Bivariate Analysis: This analysis is related to cause and the relationship between the two attributes. We will try to understand the dependence of attributes on each other.

Multivariate Analysis: This is done when more than two variables have to be analysed simultaneously.

Data Cleaning: We shall clean the dataset and handle the missing data, outliers, and categorical variables.

Testing Hypothesis: We shall check if our data meets the assumptions required by most of the multivariate techniques.
