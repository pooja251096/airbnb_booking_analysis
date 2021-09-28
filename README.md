# airbnb_booking_analysis

# Table of Contents
1. Installation
2. Introducing a Dataset
3. Project Motivation
4. Data Preparation
5. File Description
6. Results

# Installation
For running this project, the most important library is Python version of Anaconda Distribution. It installs all necessary packages for analysis and building models.

# Introducing a Dataset
Data for analyzing trends in Boston's Airbnb is available for free in Kaggle.com and here.
This dataset contains data on listings with a huge number of features, user's reviews and calendar info for Airbnb homes in Boston.

# Project Motivation
I chose this project to understand the trends of Airbnb in Boston area and analysis is done through addressing the following questions.
	1. How well can we predict a listing's price and what features correlate well with the pricing?
  2. Where to invest in a property in Boston to get the maximum number of returns from Airbnb?
	3. How well can we predict reviews and what aspects are correlated with the reviews?

# Data Preparation
This dataset has 3,585 observations and 95 features. The target features for analysis are price, review_scores_rating. To proceed with the analysis,
data wrangling should be done as this data set is really messy.
1. I had to clean up the values in several columns: the price column had a dollar sign ($) and comma (,) characters and was in object format. I removed these so
 	 the data can be translated into an integer.
2. The data types for other columns like the number of bedrooms, bathrooms, accommodates also required a change so they can be used in calculations.
3. Few columns such as neighbourhood_group_cleansed, jurisdiction_names, license, has_availability were dropped from the dataset as there were no recordings
   associated with them. These were all empty columns present in the data.
4. City column had a lot of duplicate entries with few case-sensitive entries, space addition issues, etc. All replicates were replaced with a single city code name and 
	 this cleaned data was put into a new column called city_cleansed in listings data. City column also had an unusual entry in some native language which was considered 
	 for dropping because there was only one entry as such and I was not losing so much data dropping it.
	 
# File Descriptions
There is a notebook available here to showcase work related to the above questions and wrangling process. There are 3 data files used to address the above qustions
1. Airbnb_EDA_Capstone_Project.ipynb - colab notebook
2. Airbnb.pdf - Presentation file 

# Result
Exploratory Data Analysis successfully done on this dataset and obtained few good inferences




