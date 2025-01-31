Sentiment Analysis on Twitter Data
Introduction
Social media, especially Twitter, is a goldmine of public opinion. Whether it’s about brands, politics, entertainment, 
or global events, people freely share their thoughts, making Twitter data valuable for sentiment analysis.
This project analyzes 74,683 tweets categorized into 39 different topics to understand how people feel about various subjects.
The goal is to build a machine learning model that can classify tweets as positive, negative, or neutral. 
We’ll use TextBlob for sentiment scoring and train a Multinomial Naïve Bayes classifier to improve accuracy. 
By the end of the project, we’ll have a system that can automatically determine sentiment from Twitter data.
________________________________________
Project Overview
1. Data Import
The dataset comes from Kaggle, where tweets from 39 different topics are consolidated. We load the data into a Pandas DataFrame for further processing.
2. Data Cleaning
Before analysis, we clean the dataset by:
✅ Removing duplicate tweets to avoid bias.
✅ Stripping unnecessary spaces from text.
✅ Replacing null values with NaN for proper handling.
✅ Filtering tweets related to Amazon for a focused study.
3. Text Preprocessing
To prepare the data for sentiment analysis, we:
🔹 Tokenize tweets (split them into words).
🔹 Remove stopwords (like the, is, and).
🔹 Normalize text (convert to lowercase, remove special characters).
4. Sentiment Analysis with TextBlob
We use TextBlob, a Python NLP library, to analyze sentiment. It assigns two values:
✔ Polarity: Measures sentiment (ranges from -1 = negative to +1 = positive).
✔ Subjectivity: Determines if a tweet is opinion-based or factual.
5. Machine Learning Model (Multinomial Naïve Bayes)
To improve sentiment classification, we train a Multinomial Naïve Bayes (MNB) model:
📌 We split the dataset into training and testing sets.
📌 Train the model on processed tweets.
📌 Predict sentiment on new tweets.
6. Model Evaluation
We measure the model’s performance using:
📊 Accuracy Score – how well the model predicts sentiment.
📊 Classification Report – precision, recall, and F1-score.
📊 Confusion Matrix – a breakdown of correct vs. incorrect predictions.
7. Data Visualization
Finally, we visualize our results using matplotlib and seaborn:
📌 Sentiment distribution across different topics.
📌 Word clouds showing frequently used words in positive and negative tweets.
________________________________________
Conclusion
This project builds a practical sentiment analysis system using real Twitter data. By combining TextBlob's sentiment scoring with a Naïve Bayes classifier, 
we can analyze how people feel about different topics. This approach can be extended to monitor brand reputation, analyze customer feedback, 
or track public sentiment on social issues.

