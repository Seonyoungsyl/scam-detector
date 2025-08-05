# Scam Detector

Developed a scam detector for SMS messages that automatically identifies whether a given message is ham/normal, spam, or smishing through employing 3 different supervised machine learning models, which are Random Forest, Decision Tree, and Linear Regression models.
Here is a basic website that employs our model to classify messages: https://scamdetectorpublic-1.streamlit.app/

## Problem Statement <!--- do not change this line -->

As technology continues to evolve, it’s becoming increasingly difficult for older generations and those with limited exposure to technology to identify scam messages. At the same time, scammers are taking advantage of digital platforms to commit fraud more easily. One major concern is the rise in scam messages, which has grown significantly. To address this issue, we’ve decided to build a model that can detect and flag scam messages automatically.

## Key Results <!--- do not change this line -->

Developed models using supervised machine models:
1. Random Forest
   - 95.8 % accuracy
   - Out of 115 smishing-detected messages, 105 actual smishings
   - Out of 89 spam-detected messages, 71 actual spams
2. Logistic Regression
   - 95.7% accuracy
   - Out of 117 smishing-detected messages, 107 actual smishings
   - Out of 81 spam-detected messages, 69 actual spams
4. Decision Tree
   - 94.1% accuracy
   - Out of 122 smishing-detected messages, 101 actual smishings
   - Out of 84 spam-detected messages, 64 actual spams

Accuracies of models using Logistic Regression and Random Forest are higher than the one using Decision Tree. 
This may be because Decision Tree is more susceptible to outliers compared to Logistic Regression and Random Forest
Structurally, Random Forest is a combination of multiple Decision Trees so it is more robust than just one Decision Tree. 
But it was 5% worse than Logistic Regression when detecting spams
Logistic Regression is better to detect the spam-only class while Random Forest is more accurate across all 3 classes.

## Methodologies <!--- do not change this line -->

To accomplish this, we cleaned the dataset we have chosen by removing unnecessary columns and converting texts into binary and vectors.
Our team trained the model with 4784 messages and tested it with 1197 unseen messages to avoid overfitting. We have developed 3 models, 
each employing a different type of supervised machine learning model detailed above in the Key Results section.


## Data Sources <!--- do not change this line -->

SMS Phishing Dataset for Machine Learning and Pattern Recognition by Mendeley Data: *https://data.mendeley.com/datasets/f45bkkt8pr/1* 
(5971 labeled SMS messages)

## Technologies Used <!--- do not change this line -->

- Python
- pandas
- numpy
- seaborn
- sklearn
- matplotlib


## Authors <!--- do not change this line -->

*This project was completed in collaboration with:*
- Seonyoung Lee [*joysyl0210@gmail.com*]
- Ruth Chane [*chaner@whitman.edu*]
- Rupashi Bahl [*rupashi.bahl@sjsu.edu*]
- Datt Patel [*dattpatel047@gmail.com*]
