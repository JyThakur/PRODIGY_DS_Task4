# Twitter Sentiment Analysis using NLP

## Introduction
This project focuses on performing sentiment analysis on a Twitter dataset to classify tweets into categories such as Positive, Negative, Neutral, and Irrelevant. Sentiment analysis helps in understanding public opinion and extracting insights from vast amounts of textual data shared on social media platforms like Twitter.

## Objective
The primary objective of this project is to apply Natural Language Processing (NLP) techniques to analyze the sentiments expressed in tweets. Specifically, the project aims to:
- Preprocess tweet text to remove noise and enhance model performance.
- Perform traditional sentiment analysis using labeled data.
- Implement NLP-based sentiment analysis using TextBlob.
- Compare traditional sentiment labels with NLP-based predictions.
- Visualize the distribution of sentiments and polarity scores.
- Identify tweets with extreme sentiments for qualitative insights.

## Steps Conducted
1. **Data Loading and Exploration:**
   - Loaded the dataset containing tweets, their IDs, entities, and labeled sentiments.
   - Dropped rows with missing values to ensure data quality.

2. **Data Preprocessing:**
   - Cleaned tweets by removing URLs, special characters, numbers, and extra spaces.
   - Converted text to lowercase for consistency.

3. **Traditional Sentiment Analysis:**
   - Analyzed the distribution of sentiment labels provided in the dataset.
   - Visualized the sentiment distribution using bar plots.

4. **NLP-Based Sentiment Analysis:**
   - Used TextBlob to compute the polarity score for each tweet:
     - Positive sentiment if polarity > 0.
     - Negative sentiment if polarity < 0.
     - Neutral sentiment if polarity = 0.
   - Created a new column to store the NLP-based sentiment predictions.

5. **Comparison of Traditional and NLP-Based Analysis:**
   - Compared traditional sentiment labels with NLP-based predictions.
   - Visualized the comparison using stacked bar plots.

6. **Sentiment Score Analysis:**
   - Extracted sentiment polarity scores to understand the intensity of emotions.
   - Visualized the distribution of sentiment scores using histograms.
   - Summarized sentiment scores with statistical measures like mean, standard deviation, minimum, and maximum.

7. **Extreme Sentiments:**
   - Identified and displayed the top 5 most positive and negative tweets based on polarity scores.

## Results
- Traditional sentiment labels and NLP-based predictions showed some degree of alignment, though not perfect.
- Sentiment score distribution indicated a slight positive bias in the dataset, with a mean score of 0.0767.
- Extreme sentiment tweets highlighted the strongest emotional expressions, both positive and negative.

## Conclusion
This project successfully applied NLP techniques to perform sentiment analysis on Twitter data. It demonstrated the effectiveness of combining traditional sentiment analysis with automated methods like TextBlob for a deeper understanding of textual data.

---
Feel free to explore the code, tweak the model, and visualize the results further. Contributions and feedback are welcome!

**Tools Used:** Python, Pandas, TextBlob, Matplotlib, Seaborn, Sklearn.

**Author:** [Jay Thakur]
