# ChatGPT Reviews Analysis

## Project Overview

This project analyzes ChatGPT user reviews using Python to understand user ratings, sentiment, common keywords, and changes in review activity over time.

The analysis was performed in Google Colab using Pandas, Matplotlib, TextBlob, and Scikit-learn.

## Objectives

- Analyze the distribution of user ratings.
- Classify written reviews as positive, neutral, or negative.
- Identify frequently used words in positive and negative reviews.
- Analyze monthly sentiment trends.
- Examine monthly average star ratings.

## Dataset

The dataset contains 196,727 records and four columns:

- **Review Id:** Identifier for each review.
- **Reviews:** Written user feedback.
- **Ratings:** User star rating.
- **Review date:** Date and time of the review.

The dataset covers the period from July 25, 2023, to August 23, 2024. Six records did not contain usable review text.

## Tools and Technologies

- Python
- Google Colab
- Pandas — data loading and preparation
- Matplotlib — charts and visualizations
- TextBlob — sentiment polarity analysis
- Scikit-learn — keyword frequency analysis

## Methodology

1. Loaded and inspected the CSV dataset.
2. Standardized column names and prepared ratings, dates, and review text.
3. Analyzed the distribution of star ratings.
4. Used TextBlob polarity scores to classify reviews as positive, neutral, or negative.
5. Compared average ratings across sentiment categories.
6. Used CountVectorizer to identify frequently occurring words in positive and negative reviews.
7. Grouped reviews by month to analyze sentiment counts and average ratings.

## Key Findings

- **Total records:** 196,727
- **Average star rating:** 4.50 out of 5
- **Positive sentiment:** 73.99%
- **Neutral sentiment:** 22.81%
- **Negative sentiment:** 3.21%
- **Average rating for positive reviews:** 4.69
- **Average rating for neutral reviews:** 4.16
- **Average rating for negative reviews:** 2.53

The results suggest generally favorable feedback in this dataset. The keyword and monthly trend analyses provide additional ways to explore user feedback.

## Limitations

TextBlob provides an automated estimate of sentiment and may not fully understand sarcasm, context, or complex language. Frequently occurring words also need contextual interpretation. Monthly review counts can change because the total volume of reviews changes.

## How to Run

1. Open the notebook `ChatGPT_Reviews_Analysis.ipynb` in Google Colab.
2. Upload the `chatgpt_reviews.csv` dataset to the Colab session.
3. Run the notebook cells in order.

The CSV dataset must be available in the Colab session at `/content/chatgpt_reviews.csv`, as expected by the notebook.

## Conclusion

This project demonstrates how Python can be used to prepare review data, analyze ratings and sentiment, identify frequently used words, and visualize trends over time.

The analysis provides a starting point for understanding user feedback and identifying areas for further investigation.
