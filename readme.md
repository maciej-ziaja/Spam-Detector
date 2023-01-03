## 👨‍💻 Built with
![Python](https://img.shields.io/badge/Python-FFD43B?style=for-the-badge&logo=python&logoColor=blue)
![Jupyter Notebook](https://img.shields.io/badge/Jupyter-F37626.svg?&style=for-the-badge&logo=Jupyter&logoColor=white)
![Pandas](https://img.shields.io/badge/Pandas-2C2D72?style=for-the-badge&logo=pandas&logoColor=white)
![Scikit Learn](https://img.shields.io/badge/scikit--learn-%23F7931E.svg?style=for-the-badge&logo=scikit-learn&logoColor=white)
![Matplotlib](https://img.shields.io/badge/Matplotlib-%23666666.svg?style=for-the-badge&logo=Matplotlib&logoColor=black)
## 🔍  Description

Data used in this project: [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/SMS+Spam+Collection)

The TSV file contains over 5000 text messages.
File has two columns:
```bash
message_type
text_message
```
The object of this project is to create a simple anti-spam detector for text messages.

It consists of four parts:
1. Introduction with some data transformations, quick exploratory data analysis and visualizations.
2. Training data model and using machine learning to predict whether a text message is spam or not.
3. Optimizing the process to increase performance of the model.
4. Conclusions

## 📝 Introduction and Analysis:

**Introduction**  

To handle collected data I used Jupyter Notebook with libraries:
- Pandas
- String
- Seaborn
- Matplotlib
- SKLearn
- NLTK

Collected data is a TSV file. It can be read with Pandas and turned into a Data Frame.  
There are no missing values in any of the columns.

**Exploratory Data Analysys**

- adding a column with length of the message
- boxplot - visualizing the spread of messages length
- histogram - distribution of the message length
- histograms - distribution of the message length by the message type

## 📊 Prediction with machine learning model:

**Vectorizing**

- removing the punctuation from the messages
- using CountVectorizer from SKLearn package

**Training a model**

- using the Naive Bayes model
- evaluating the model

This method reached **96.53%** accuracy.

## 🛍️ Optimizing the process:

**Vectorizing**

- removing the punctuation from the messages
- removing the stopwords using NLP package
- using CountVectorizer from SKLearn package
- applying TF-IDF

**Training a model**

- using the Naive Bayes model
- evaluating the model

This method reached **95.75%** accuracy.

**Changing the model to Random Forest**

- using the Random Forest model
- evaluating the model

This method reached **97.37%** accuracy.


## 📋 Conclusions 


There is a lot of optimization possibilities to try with this project. 

Firstly, there are lots of other text pre-processing techniques that can be applied to messages before vectorizing it (such as ['stemming'](https://en.wikipedia.org/wiki/Stemming)).  

Secondly, there is a lot different classifiers that can prove to be more efficient in this specific situation.  

Also, deep understanding of the data can help to know what results should be achieved.