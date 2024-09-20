# Information Sharing in Seaweed Farming: Investigating the Dynamics of Participation in Facebook Groups Among Indonesian Seaweed Farmers

## Context

Seaweed farming is an important source of income for Indonesia's coastal communities. However, Indonesian seaweed farmers face challenges such as price transparency, market access, and access to quality seedlings. Like many other small-scale producers, they live at subsistence levels. 

There is growing academic interest in the use of online information sharing platforms to improve seaweed farmer livelihoods, such as through increased price transparency and access to larger markets. This project analyzes the trends in the most commonly discussed topics on Facebook, a popular platform used by seaweed farmers, in an attempt to understand how seaweed farmers utilize current technologies. 

**Understanding what seaweed farmers post about, i.e. what issues they face at different points throughout the year, is critical not only in academic discussions around digital technology empowerment, but also aquaculture extension policy, and how governments can better cater towards small aquaculture farmers that are the backbone of Indonesia's economy.**

## Project Overview & Objectives

This project analyzes Facebook posts from Indonesian seaweed farmers to uncover patterns in what farmers are interested in and its relationships with environmental factors, such as weather conditions. The dataset is comprised of posts from the Rumput Laut Centre, one of the largest seaweed farming Facebook groups at approximately 56,000 members. This project was created for the final DATASCI112 project at Stanford University. 


## Data Description

The source of the Facebook posts is from Madeline Grist's thesis, *Propagule Distribution Systems of Tropical Carrageenan Seaweed in South Sulawesi: Value Chain and Social Media Analyses* and while the dataset is not publicly available, the Facebook group from which the posts were gleaned is a public Facebook group, the Rumput Laut Centre. 

The dataset includes posts collected between September 1, 2021, and August 29, 2022. I then joined weather and climatic data from Meteostat, which provides open weather and climate data. I used weather data from Makassar, a city near Indonesia’s largest seaweed farming hotspot.    

This tabular dataset consists of rows, each representing a Facebook post, and columns that capture various features associated with each post. These features include the text of the post in Bahasa Indonesia, English, and a processed English format (stemmed, lemmatized, and other NLTK operations), as well as the category of the post, the date it was published, and relevant weather features from the day of the post, such as precipitation and temperature.

The weather data is available [here](https://meteostat.net/en/place/id/makassar?s=97180&t=2022-08-04/2022-09-01).

## Methodology
### 1. Data Cleaning
- Cleaning the English text in preparation for Latent Dirichlet Allocation (LDA)
 - Standard text cleaning procedures such as *lowercasing, removing special characters, stopwords, and punctuation, and stemming* to reduce words to their base or root form.

### 2. Data Merging
- Incorporating environmental effects by joining weather data for the same period
 - Includes metrics like *average temperature, precipitation, and wind direction* and was sourced from Meteostat.

### 3. Analysis 
- Performing unsupervised clustering using Latent Dirichlet Allocation (LDA) on the cleaned text data
 - Helps identify latent topics within the posts, which were then analyzed to understand their correlation with various environmental factors.

**The hypothesis was that certain types of posts, such as those related to buying or selling seaweed, might correlate with weather patterns, particularly precipitation levels, which influence seaweed productivity.**

### Quality Assessment of Clusters
- The quality of the clusters generated from LDA was assessed using a **K-nearest classifier model.** This model was trained to predict the correct category of posts based on the clusters identified. 
 - Cross-validation was used to evaluate the model, with the f1_macro score chosen as the evaluation metric due to its balance of precision and recall

### Visualization
- Graphed the popularity of various seaweed farming topics over time (e.g. Seaweed Information, Buying and Selling Seaweed, etc).
- Plotted number of posts in each cluster against precipitation and average temperature
- Created word clouds highlighting common words and themes in different clusters
- Created a confusion matrix to assess quality of clusters

## Results & Analysis

**The following word clouds show common words found in a sample of the clusters.**
<img width="1113" alt="Screenshot 2024-09-20 at 11 58 27 AM" src="https://github.com/user-attachments/assets/1055fc28-ed7d-4e7a-8e17-d9947f7b8140">

**The following graph shows trends in which themes were more commonly discussed each month. August had the greatest number of Facebook posts, with spikes in February and March.**

Other studies indicate that tropical seaweed grows well in dry season, which is between May and October for Sulawesi (where the majority of Indonesian seaweed is grown). The results from this data indicate a greater number of posts during dry season, which suggest that seaweed farmers use Facebook more when there is increased seaweed growth. This indicates that farmers are using Facebook to assist in their seaweed related activities.

<img width="967" alt="Screenshot 2024-09-20 at 11 59 56 AM" src="https://github.com/user-attachments/assets/de8eb888-a13a-4ded-8910-44c0ed48c74d">

**The two graphs below indicate that there is not a significant difference between topics discussed in seaweed farming Facebook groups given different temperatures and levels of precipitation, likely due to the fact that precipitation and temperature are highly location dependent, and the members of the Facebook group could be from vastly different locations**

<img width="1107" alt="Screenshot 2024-09-20 at 12 01 24 PM" src="https://github.com/user-attachments/assets/15093044-b311-410f-98aa-39c3edd6c268">

**The confusion matrix below is used to assess the distinctiveness of each cluster. The cluster titled "Local Updates" seems to be an amalgamation of the other clusters, so in future extrapolations of this project, I would look into the posts in that cluster and test a semi-supervised approach to tease out patterns within "Local Updates".**

<img width="492" alt="Screenshot 2024-09-20 at 12 17 43 PM" src="https://github.com/user-attachments/assets/992b1d91-90ae-4271-9949-8b584fd7e565">


## Next Steps / Other Considerations
- To improve the f1_macro score, any future extension of this project should consider using a semi-supervised approach such as seeded or guided LDA.


## Featured Deliverable
* [Presentation Poster](https://docs.google.com/presentation/d/1UJeXbBqSDElVRAl0k35jpL8aX3qRYpi1Cq2KkW9ZmJ0/edit?usp=sharing)


** Researcher Contact : [Kaylee Shen](https://github.com/[[kayshen1120]]) (kayshen@stanford.edu)**



