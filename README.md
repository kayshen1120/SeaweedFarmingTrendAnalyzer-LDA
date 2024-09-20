# Information Sharing in Seaweed Farming: Investigating the Dynamics of Participation in Facebook Groups Among Indonesian Seaweed Farmers

## Context

Seaweed farming is an important source of income for Indonesia's coastal communities. However, Indonesian seaweed farmers face challenges such as price transparency, market access, and access to quality seedlings. Like many other small-scale producers, they live at subsistence levels. 

There is growing academic interest in the use of online information sharing platforms to improve seaweed farmer livelihoods, such as through increased price transparency and access to larger markets. This project analyzes the trends in the most commonly discussed topics on Facebook, a popular platform used by seaweed farmers, in an attempt to understand how seaweed farmers utilize current technologies. 

## Project Overview & Objectives

(say data science project from 112 here)


This project analyzes Facebook posts from Indonesian seaweed farmers to uncover patterns in what farmers are interested in and relationships with environmental factors such as weather conditions. The dataset is comprised of posts from the Rumput Laut Centre, one of the largest seaweed farming Facebook groups at approximately 56,000 members, collected between September 1, 2021, and August 29, 2022.

This data science project focuses on analyzing Facebook posts from Indonesian seaweed farmers to uncover patterns and relationships with environmental factors such as weather conditions. 

Data science project to analyze themes in seaweed farming Facebook posts over time to understand issues farmers face for better policy making &amp; the potential for digital technology usage in aquacultural extension services. Created in part for my honors thesis project and in part for the final DATASCI112 project at Stanford University. 


Text Analysis: Perform text cleaning and Latent Dirichlet Allocation (LDA) for unsupervised clustering of the posts.
Environmental Correlation: Explore potential correlations between the clustered themes in the posts and environmental variables like temperature and precipitation.

## Data Description

The source of the Facebook posts is from Madeline Grist's thesis, *Propagule Distribution Systems of Tropical Carrageenan Seaweed in South Sulawesi: Value Chain and Social Media Analyses* and while the dataset is not publicly available, the Facebook group from which the posts were gleaned is a public Facebook group, the Rumput Laut Centre. 

The dataset includes posts collected between September 1, 2021, and August 29, 2022. I then joined weather and climatic data from Meteostat, which provides open weather and climate data. I used weather data from Makassar, a city near Indonesia’s largest seaweed farming hotspot.    

This tabular dataset consists of rows, each representing a Facebook post, and columns that capture various features associated with each post. These features include the text of the post in Bahasa Indonesia, English, and a processed English format (stemmed, lemmatized, and other NLTK operations), as well as the category of the post, the date it was published, and relevant weather features from the day of the post, such as precipitation and temperature.

The weather data is available [here](https://meteostat.net/en/place/id/makassar?s=97180&t=2022-08-04/2022-09-01).

## Methodology

A description of the methods used for the analysis or modeling.
Explanation of the approach, including key algorithms, techniques, or tools employed.
Mention any assumptions made or challenges faced in the project.

Google Colab: For executing Python notebooks in a cloud-based environment.
Python Libraries:
pandas for data manipulation.
matplotlib and seaborn for data visualization.
sklearn for implementing LDA.
Data Sources:
Facebook posts from Rumput Laut Centre.
Weather data from Meteostat.
Project Structure
Data Importation: Load data from Google Drive.
Data Cleaning: Clean the text data to prepare for LDA.
Text Clustering: Use LDA to cluster posts and analyze the clusters.
Weather Data Incorporation: Integrate weather data to explore environmental impacts on post content.
Analysis: Investigate correlations between post clusters and weather conditions.
Installation and Setup
Clone the project repository:

* Inferential Statistics
* Machine Learning
* Data Visualization
* Predictive Modeling
* etc.

## Results & Analysis

(base this off of the project poster)


## Next Steps / Other Considerations
"""
 (NEXT TIME TO DO A GUIDED LDA)
To guide an LDA (Latent Dirichlet Allocation) model to include certain words in different topics,
you can use a semi-supervised approach known as "seeded" or "guided" LDA. This involves incorporating
seed words or a dictionary of seed words for each topic, which influences the topic-word distributions.

One method to achieve this is to use the GuidedLDA library, which allows you to incorporate prior
knowledge into the LDA model. You can specify seed words for each topic, and the model will give higher
probability to these words in the respective topics.
"""


## Featured Deliverable
* [Presentation Poster](https://docs.google.com/presentation/d/1UJeXbBqSDElVRAl0k35jpL8aX3qRYpi1Cq2KkW9ZmJ0/edit?usp=sharing)


** Researcher Contact : [Kaylee Shen](https://github.com/[[kayshen1120]]) (kayshen@stanford.edu)**



