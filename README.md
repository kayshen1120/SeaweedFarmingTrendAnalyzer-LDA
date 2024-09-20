# Information Sharing in Seaweed Farming: Investigating the Dynamics of Participation in Facebook Groups Among Indonesian Seaweed Farmers

installation and usage instructions, license and contributing information, and credits


## Context

Seaweed farming is an important source of income for Indonesia's coastal communities. However, Indonesian seaweed farmers face challenges such as price transparency, market access, and access to quality seedlings. Like many other small-scale producers, they live at subsistence levels. 

There is growing academic interest in the use of online information sharing platforms to improve seaweed farmer livelihoods, such as through increased price transparency and access to larger markets. This project analyzes the trends in the most commonly discussed topics on Facebook, a popular platform used by seaweed farmers, in an attempt to understand how seaweed farmers utilize current technologies. 

## Project Overview & Objectives

This project analyzes Facebook posts from Indonesian seaweed farmers to uncover patterns in what farmers are interested in and its relationships with environmental factors, such as weather conditions. The dataset is comprised of posts from the Rumput Laut Centre, one of the largest seaweed farming Facebook groups at approximately 56,000 members. This project was created for the final DATASCI112 project at Stanford University. 


## Data Description

The source of the Facebook posts is from Madeline Grist's thesis, *Propagule Distribution Systems of Tropical Carrageenan Seaweed in South Sulawesi: Value Chain and Social Media Analyses* and while the dataset is not publicly available, the Facebook group from which the posts were gleaned is a public Facebook group, the Rumput Laut Centre. 

The dataset includes posts collected between September 1, 2021, and August 29, 2022. I then joined weather and climatic data from Meteostat, which provides open weather and climate data. I used weather data from Makassar, a city near Indonesia’s largest seaweed farming hotspot.    

This tabular dataset consists of rows, each representing a Facebook post, and columns that capture various features associated with each post. These features include the text of the post in Bahasa Indonesia, English, and a processed English format (stemmed, lemmatized, and other NLTK operations), as well as the category of the post, the date it was published, and relevant weather features from the day of the post, such as precipitation and temperature.

The weather data is available [here](https://meteostat.net/en/place/id/makassar?s=97180&t=2022-08-04/2022-09-01).

## Methodology
### Data Cleaning
The first step in the preprocessing was cleaning the English text in preparation for Latent Dirichlet Allocation (LDA). This involved standard text cleaning procedures such as lowercasing, removing special characters, stopwords, and punctuation, and stemming to reduce words to their base or root form.

### Data Enrichment
To incorporate environmental effects, weather data for the same period was integrated into the analysis. This data included metrics like average temperature, precipitation, and wind direction and was sourced from Meteostat.

### Analysis Methodology
Unsupervised clustering using Latent Dirichlet Allocation (LDA) was performed on the cleaned text data. This method helped identify latent topics within the posts, which were then analyzed to understand their correlation with various environmental factors. The hypothesis was that certain types of posts, such as those related to buying or selling seaweed, might correlate with weather patterns, particularly precipitation levels, which influence seaweed productivity.

### Quality Assessment of Clusters
The quality of the clusters generated from LDA was assessed using a K-nearest classifier model. This model was trained to predict the correct category of posts based on the clusters identified. Cross-validation was used to evaluate the model, with the f1_macro score chosen as the evaluation metric due to its balance of precision and recall. The performance of the model provided insights into the distinctiveness and relevance of the clusters.

### Visualization
Several visualizations were created to better understand the relationship between cluster distribution and climate-related variables:

Graphs plotting the number of posts in each cluster against precipitation, average temperature, and wind direction.
Word clouds were generated for each cluster to visualize the most common words and themes within each group, enhancing the interpretability of the LDA results.


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



