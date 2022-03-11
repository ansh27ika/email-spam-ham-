# email-spam-ham-
## email-spam-ham classification

# overview>>
>>spam:
Internet Spam is a collection of irrelevant texts sent in the form of messages or email, 
with the motive of promoting stuff, advertisements of websites that support online dating,
pornography, and also phishing and spreading viruses.
This spam, if accidentally or intentionally clicked by you, 
can lead to your system being damaged by virus attacks,
wastage of your network resources, and also a waste of time.
>>Ham:
"Ham" is e-mail that is not Spam. In other words, "non-spam", or "good mail".
This looks like a normal email reply to another person,
which is not difficult to classified as a ham:

1.EDA (Exploratory data analysis)
2.Data Preprocessing
3.Feature Extraction
4.Scoring & Metrics



>> importing important librarires
import numpy as np 
import pandas as pd 
from sklearn.model_selection import train_test_split
from sklearn.feature_extraction.text import TfidfVectorizer
from sklearn.linear_model import LogisticRegression 
from sklearn.metrics import accuracy_score

 
>>columns in dataset ([5572 rows x 2 columns])
1. Category	
2. Message


>> training of model 
used logistic regression


>>Train Test Split
It is important to split your data set to training set and test set, 
so that you can evaluate the performance of your model using the test set 
before deploying it in a production environment.

>>Data Preprocessing
Text Cleaning  is a very important step in machine learning 
because your data may contains a lot of noise and unwanted character
 such as punctuation, white space, numbers, hyperlink and etc.


observation:
it can detect and filter out spam and phishing emails with about 99.9 percent accuracy. 
The implication of this is that one out of a thousand messages succeed in evading their email spam filter.
