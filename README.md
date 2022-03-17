# Email-Spam-Ham
#### classification model

# Overview
#### SPAM:
Internet Spam is a collection of irrelevant texts sent in the form of messages or email, 
with the motive of promoting stuff, advertisements of websites that support online dating,
pornography, and also phishing and spreading viruses.
This spam, if accidentally or intentionally clicked by you, 
can lead to your system being damaged by virus attacks,
wastage of your network resources, and also a waste of time.
#### HAM:
"Ham" is e-mail that is not Spam. In other words, "non-spam", or "good mail".
This looks like a normal email reply to another person,
which is not difficult to classified as a ham:
##### STEPS TO BE FOLLOWED
1.EDA (Exploratory data analysis)
2.Data Preprocessing
3.Feature Extraction
4.Scoring & Metrics



### Importing librarires
1. `numpy` 
2. `pandas` 
3.  `train_test_split`
4.  `TfidfVectorizer`
5.  `xgboost`
6. `accuracy_score`
7. `pickle`


 
## columns in dataset [5572 rows x 2 columns]
1. Category	
2. Message

### Data Preprocessing
Text Cleaning  is a very important step in machine learning 
because your data may contains a lot of noise and unwanted character
such as punctuation, white space, numbers, hyperlink and etc.
* Lower case
* Tokenization
* Removing special characters
* Removing stop words and punctuation
* Stemming

### What is NLTK?
NLTK is a toolkit build for working with NLP in Python. It provides us various text processing libraries with a lot of test datasets. 
A variety of tasks can be performed using NLTK such as tokenizing, parse tree visualization, etc

## CountVectorizer and TfidVectorizer 
TfidfVectorizer and CountVectorizer both are methods for converting text data into vectors as model can process only numerical data.
In CountVectorizer we only count the number of times a word appears in the document which results in biasing in favour of most frequent words.
##### Train Test Split
It is important to split your data set to training set and test set, 
so that you can evaluate the performance of your model using the test set 
before deploying it in a production environment.


## DEPLOYMENT 
### Post Url
http://127.0.0.1:8080/predict
### Body Response
{"Message":"Nah I don't think he goes to usf, he lives around here though"}
### Prediction
spam


