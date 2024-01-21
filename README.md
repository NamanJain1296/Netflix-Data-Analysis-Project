# Netflix Data Analysis Project

## Overview

Welcome to the Netflix Data Analysis project! This project explores the extensive Netflix dataset, providing insights into user preferences, content trends, and sentiment analysis of user reviews. Leveraging the power of data science and analytics, we aim to uncover intriguing patterns and trends within the Netflix library.

## Features

- **Distribution of Content Rating:** Explore the distribution of content ratings to understand the audience preferences and overall content landscape.
  
- **Top 10 Actors and Directors:** Identify the most influential actors and directors based on their involvement in Netflix content.

- **Content Distribution:** Identify the countries that produced maximum content till date for Netflix.

- **Sentiment Analysis with TextBlob:** Utilize TextBlob, a powerful natural language processing library, for sentiment analysis on user reviews. Understand the overall sentiment of user feedback and comments.

- **Content Analysis:** Dive into the dataset to analyze content based on various attributes, such as genres, categories, and more.

## Analysis Tools

- Python for data cleaning, manipulation, and analysis.
- Pandas and NumPy for data processing.
- Matplotlib and Seaborn for data visualization.
- Plotly Express for interactive and engaging visualizations.
- TextBlob for sentiment analysis.

## Sentiment Analysis

### Using TextBlob

In this project, we employ TextBlob, a Python library for processing textual data. TextBlob makes it easy to perform sentiment analysis, extracting subjective information from user reviews and comments.

```python
# Example code snippet for sentiment analysis with TextBlob
from textblob import TextBlob

# Assuming 'reviews' is a column in your DataFrame containing user reviews
df['sentiment'] = df['reviews'].apply(lambda x: TextBlob(str(x)).sentiment.polarity)
