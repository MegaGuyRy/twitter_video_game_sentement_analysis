# Twitter Video Game Sentement Analysis

## Table of Contents
- [Overview](#overview)
- [Data Sources](#Data-Sources)
- [Tools](#Tools)
- [Data Cleaning](#Data-Cleaning)
- [Exploratiry Data Analysis](#Exploratiry-Data-Analysis)
- [Data Analysis](#Data-Analysis)
- [References](#References)

### Overview
This was my final project for my Natural Language Processing course. I used labled twitter data that was catagorizing by the subject and as a positive neutral or negitive tweets. This was used to train a naive bayes classifier and identify common words associated with negitive or positive sentiments.

### Data Sources
The dataset I reference for this project is from Kaggle and is a collection of tweets it was compiled in the year 2022. The data contains 12447 unique entried and has four features:
- ID
- Catagory/Game
- Sentiment
- Tweet

### Tools
- Excel: initial exploration, manual cleaning, calculate and store new data.
- Python: (Pandas, NumPy, Matplotlib, NLTK, Sklearn) – data wrangling, data cleaning, data visualization, and model building.

### Data Cleaning
In the initial data cleaning process I used python to removed all rows with null entries. I then nomalized all comlumns so all strings were lowercase as well as removing punctuation, links and @'s in the tweets column. This greatly reduced the number of token that would need be analysed will preserving the integrity of the data.

<img width="162" alt="image" src="https://github.com/user-attachments/assets/168b4456-768a-4621-ad61-abcf33e1fa20" />

### Exploratiry Data Analysis
EDA Reviled that the data held:
1. There are 32 unique catagories in the data.
<img width="166" alt="image" src="https://github.com/user-attachments/assets/426f5220-6b9b-4a6a-841c-2fe92d2ea249" />

2. Each catagory contains roughly 400 tweets pretaining to it.
<img width="176" alt="image" src="https://github.com/user-attachments/assets/d913c4f0-673e-4764-b670-53781e265b1f" />

3. Created an ordered list of of the catagories based on the distribution of positive and negative tweets.
<img width="313" alt="image" src="https://github.com/user-attachments/assets/818c1810-6457-4311-a8c8-1cb0e01ddf0b" />

4. Establish the most frequent words to appear in positive tweets.
<img width="201" alt="image" src="https://github.com/user-attachments/assets/585bfa26-3e84-4e74-8b0c-fba71eaa28a1" />
<img width="602" alt="image" src="https://github.com/user-attachments/assets/d42f1e59-2cdd-41e2-9f04-7736f91a1c86" />

5. Establish the most frequent words to appear in negative tweets.
<img width="212" alt="image" src="https://github.com/user-attachments/assets/b66e4ef2-2070-4f27-ba29-9b8b5db6338f" />
<img width="616" alt="image" src="https://github.com/user-attachments/assets/ac5a9e42-693a-4e5d-a690-e4592dfc1220" />

### Data Analysis
To train my naive bayes classifier I split the data into 80% for training and 20% for testing. \

<img width="326" alt="image" src="https://github.com/user-attachments/assets/45aaec0a-5634-4809-8e94-a045eeaa06b6" />

### References
Dataset: https://www.kaggle.com/datasets/palakjain41/video-games-dataset-for-sentiment-analysis
