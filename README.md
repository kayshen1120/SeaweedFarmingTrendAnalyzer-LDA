# Information Sharing in Seaweed Farming: Investigating the Dynamics of Participation in Facebook Groups Among Indonesian Seaweed Farmers
Project Overview
This data science project focuses on analyzing Facebook posts from Indonesian seaweed farmers to uncover patterns and relationships with environmental factors such as weather conditions. The dataset includes posts from the Rumput Laut Centre collected between September 1, 2021, and August 29, 2022.

Data Description
The primary dataset consists of Facebook posts which have been scraped and stored. Additionally, weather data from Makassar (available at Meteostat) has been incorporated to analyze the impact of environmental factors on the content of the posts.

Objectives
Text Analysis: Perform text cleaning and Latent Dirichlet Allocation (LDA) for unsupervised clustering of the posts.
Environmental Correlation: Explore potential correlations between the clustered themes in the posts and environmental variables like temperature and precipitation.
Tools and Technologies Used
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

bash
Copy code
git clone <repository-url>
Install required Python packages:

bash
Copy code
pip install -r requirements.txt
Usage
To run the project, navigate to the project directory and launch the Jupyter notebook:

bash
Copy code
jupyter notebook DATASCI112_Project_Colab.ipynb
Contributors
[Your Name]: Project Lead - Responsible for data analysis and model development.
License
This project is licensed under the MIT License - see the LICENSE.md file for details.

Acknowledgments
Special thanks to Rumput Laut Centre for providing access to the data necessary for this analysis.



Data science project to analyze themes in seaweed farming Facebook posts over time to understand issues farmers face for better policy making &amp; the potential for digital technology usage in aquacultural extension services. Created in part for my honors thesis project and in part for the final DATASCI112 project at Stanford University. 

## Project Intro/Objective
The purpose of this project is ________. (Describe the main goals of the project and potential civic impact. Limit to a short paragraph, 3-6 Sentences)

### Partner
* [Name of Partner organization/Government department etc..]
* Website for partner
* Partner contact: [Name of Contact], [slack handle of contact if any]
* If you do not have a partner leave this section out

### Methods Used
* Inferential Statistics
* Machine Learning
* Data Visualization
* Predictive Modeling
* etc.

### Technologies
* R 
* Python
* D3
* PostGres, MySql
* Pandas, jupyter
* HTML
* JavaScript
* etc. 

## Project Description
(Provide more detailed overview of the project.  Talk a bit about your data sources and what questions and hypothesis you are exploring. What specific data analysis/visualization and modelling work are you using to solve the problem? What blockers and challenges are you facing?  Feel free to number or bullet point things here)

Different features include:
- date
- month
- average temperature
- precipitation (prcp)
- air pressure

"""
 (NEXT TIME TO DO A GUIDED LDA)
To guide an LDA (Latent Dirichlet Allocation) model to include certain words in different topics,
you can use a semi-supervised approach known as "seeded" or "guided" LDA. This involves incorporating
seed words or a dictionary of seed words for each topic, which influences the topic-word distributions.

One method to achieve this is to use the GuidedLDA library, which allows you to incorporate prior
knowledge into the LDA model. You can specify seed words for each topic, and the model will give higher
probability to these words in the respective topics.
"""

## Needs of this project

- frontend developers
- data exploration/descriptive statistics
- data processing/cleaning
- statistical modeling
- writeup/reporting
- etc. (be as specific as possible)

## Getting Started

1. Clone this repo (for help see this [tutorial](https://help.github.com/articles/cloning-a-repository/)).
2. Raw Data is being kept [here](Repo folder containing raw data) within this repo.

    *If using offline data mention that and how they may obtain the data from the froup)*
    
3. Data processing/transformation scripts are being kept [here](Repo folder containing data processing scripts/notebooks)
4. etc...

*If your project is well underway and setup is fairly complicated (ie. requires installation of many packages) create another "setup.md" file and link to it here*  

5. Follow setup [instructions](Link to file)

## Featured Notebooks/Analysis/Deliverables
* [Presentation Poster](https://docs.google.com/presentation/d/1UJeXbBqSDElVRAl0k35jpL8aX3qRYpi1Cq2KkW9ZmJ0/edit?usp=sharing)
* [Notebook/Markdown/Slide DeckTitle](link)
* [Blog Post](link)


## Data Source

The source of the Facebook posts is from Madeline Grist's thesis, *Propagule Distribution Systems of Tropical Carrageenan Seaweed in South Sulawesi: Value Chain and Social Media Analyses* and while the dataset is not publicly available, the Facebook group from which the posts were gleaned is a public Facebook group, the Rumput Laut Centre. 

The weather data is available [here](https://meteostat.net/en/place/id/makassar?s=97180&t=2022-08-04/2022-09-01).

** Researcher Contact : [Kaylee Shen](https://github.com/[[kayshen1120]]) (kayshen@stanford.edu)**

#### Other Members:

|Name     |  Slack Handle   | 
|---------|-----------------|
|[Full Name](https://github.com/[github handle])| @johnDoe        |
|[Full Name](https://github.com/[github handle]) |     @janeDoe    |

## Contact
* If you haven't joined the SF Brigade Slack, [you can do that here](http://c4sf.me/slack).  
* Our slack channel is `#datasci-projectname`
* Feel free to contact team leads with any questions or if you are interested in contributing!
