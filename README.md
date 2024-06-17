# The impact of the 'Literally me' cultural trope on Letterboxd film reviews: sentiment and keyword frequency analysis

## Table of Contents

1. [Introduction](#introduction)
2. [Content](#content)
3. [Conclusion](#conclusion)
4. [Links](#links)

## Introduction

The objectives of this analysis are to verify the alignment between the tone of reviews from Letterboxd and their star ratings, investigate the potential positive influence of the "Literally Me" trope's popularity on review sentiment, identify frequently occurring words, examine changes in the occurrence of trope-specific words, and compare the performance of the Vader and RoBERTa models.

## Content

- scrape_data.ipynb - data scraping procedures
- sentiment_analysis.ipynb - sentiment analysis
- google_data - folder with data from Google Trends for "literally me" trope keywords
- data - folder with reviews and results:
  - all_reviews.csv - contain all preprocessed reviews, which the whole analysis is based on
  - \*\_reviews.csv - reviews before removing duplicates and the ones that are covered with "this review may contain spoilers"
  - \*\_fixed.csv - reviews without duplicates and wrong "Review" content
  - results2.csv - results for Vader and RoBERTa based on "all_reviews.csv"
  - examples.csv - example reviews that were used for preliminary tests of RoBERTa and Vader

## Conclusions

The popularity of the 'literally me' trope is reflected in the reviews by Letterboxd users.

1. RoBERTa model demonstrated improved sentiment classification based on user ratings, indicating a shift towards more negative sentiments over the trend period.
2. There has been a noticeable transition from using 'film' to predominantly 'movie,' suggesting a shift in the seriousness of reviews on Letterboxd.
3. Keywords specific to the 'literally me' trope are notably more prevalent in recent reviews, underscoring their increasing usage in contemporary critiques.
4. RoBERTa exhibited superior sentiment recognition compared to Vader.
5. The review sentiment is consistent with the star rating

## Links

- my presentation (in polish)

  https://docs.google.com/presentation/d/1G2nYoNCjqpZu8ys1xREpiMG-lHYRKERBEcMUZ2bpX0M/edit?usp=sharing

- data scraping - Beautiful Soup documentation \[June 2024\]:

  https://beautiful-soup-4.readthedocs.io/en/latest/#making-the-soup

- usage of Vader and RoBERTa - tutorial from Rob Mulla \[June 2024\]:

  https://www.youtube.com/watch?v=QpzMWQvxXWk&ab_channel=RobMulla

- used RoBERTa models \[June 2024\]:

  https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment

  https://huggingface.co/cardiffnlp/twitter-roberta-base-sentiment-latest

- word clouds - WordCloud for Python documentation \[June 2024\]:

  https://amueller.github.io/word_cloud/

- "Literally me" characters explanation \[June 2024\]:

  https://www.youtube.com/watch?v=5e6DmT2AzQc&t=165s&ab_channel=DuCinema
