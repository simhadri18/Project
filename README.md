# Polarity Score-Based Fake and Genuine Tweet Classifier

## Project Overview
This project focuses on building a machine learning classifier to distinguish between fake and genuine tweets using Natural Language Processing (NLP) techniques. The classifier is built using TextBlob for sentiment analysis and a Decision Tree Classifier (DTC) for classifying tweets based on their polarity score.
## Dataset
The dataset consists of tweets, mainly focused on social issues like women's safety. It includes fields such as tweet text, tweet ID, length of the tweet, created_at, source, favorite_count, and retweet_count.
Preprocessing techniques like tokenization, stop word removal, and lemmatization are applied to clean the dataset.
## project steps

1. Data Preprocessing
Tokenization: Tweets are split into individual words.
Stop Word Removal: Common words with little semantic meaning are removed.
Stemming and Lemmatization: Words are reduced to their base form.
TF-IDF: Term Frequency-Inverse Document Frequency is used for feature extraction.

2. Sentiment Analysis
Using TextBlob, the polarity of each tweet is determined:
Polarity < 0: Negative (Fake Tweet)
Polarity > 0.5: Positive (Genuine Tweet)
Polarity between 0 and 0.5: Neutral

3. Classification Model
A Decision Tree Classifier (DTC) is trained on the processed features to classify tweets as fake or genuine based on their sentiment polarity.
## How to Run the Project
1. Clone the Repository:
   ```bash
   git clone https://github.com/yourusername/your-repo-name.git
   cd your-repo-name
3. Install Dependencies Install all required Python packages using the:
   ```bash
   pip install -r requirements.txt
5. Run the Main Script Launch the GUI for uploading the dataset, processing tweets, and viewing sentiment analysis results:
    ```bash
    python main.py
    
7. Explore Results:
   After loading a dataset, the GUI allows you to preprocess the data, run sentiment analysis, and generate graphs showing the distribution of fake and genuine tweets.
## Dependencies
The following libraries are used in the project:

Python 3.7+
TextBlob
NLTK
Pandas
Matplotlib
Tkinter (for GUI)
## Project Features
#### Data Cleaning: 
Preprocessing tweets by removing punctuation, stop words, and converting text to lowercase.
#### Sentiment Analysis: 
Using TextBlob to analyze the sentiment of each tweet and categorize it as positive, neutral, or negative.
#### Machine Learning Classifier: 
Decision Tree Classifier (DTC) to predict fake or genuine tweets.
#### GUI Interface: 
A user-friendly interface to upload datasets and view sentiment analysis results and performance graphs.

## Results
The Decision Tree Classifier provides predictions based on tweet polarity.
A pie chart is generated to visually display the percentage of fake and genuine tweets in the dataset.

## Future Scope
Extend the classifier to work with other social media platforms like Facebook and Instagram.
Further improve the model's accuracy by integrating advanced deep learning techniques such as LSTMs or CNNs.



