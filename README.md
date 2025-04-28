**Duplicate Question Pairs**

The streamlit app takes two questions as an input and predicts whether The questions are Duplicate or unique. This is quite useful in providing services to question and answer platform and forums such as Quora,Stack Overflow.Yahoo Answers etc.

The machine learning model was created mainly using: Bag of Words, Fuzzy features etc

**Render link of this project:**
https://duplicate-question-pair-finder.onrender.com/

**Roadmap**
I divide this project's roadmap in 5 steps.

1)Understanding the data(EDA)

Some of the insights I found are in the notebook attached in the repository.You check them there.

2)Preprocessing the data.

The data needed to be preprocessed as it had some special characters and contractions(https://en.wikipedia.org/wiki/Wikipedia%3aList_of_English_contractions)

I also used Porter stemmer and WordNetLemmatizer but later decided to drop them.

3)Modeling with only Bag of Words.

I only used tf-idf at the starting to check the accuracy.The accuracy was found to be around 73%.My main target was to reach 80%. Machine learning algorithm used was XGBoost

4)Introducing Feature Engineering.

I tried to generate some useful features such as a)Difference in lengths of these two questions. b)Mean length of the two questions.

c)Common words/min. word length between the questions

d)Common words/max. word length between the questions

e)Common words/min. word length between the questions

f)Common stop word words/min. stopword length between the questions

g)Common stop word words/max. stopword length between the questions

h)Common token word words/min. token length between the questions

i)Common token word words/max. token length between the questions

j)Is last word equal?(boolean)

k)Is first word equal?(boolean)

By applying these common features an accuracy of 77% was reached

5)Learning about Fuzzy features.

#https://www.analyticsvidhya.com/blog/2021/06/fuzzywuzzy-python-library-interesting-tool-for-nlp-and-text-analytics/

After applying these fuzzy features an accuracy of 78-79% was reached.


![dqp](https://github.com/user-attachments/assets/aeabb709-fc34-4cfe-9a1a-b6a8a73974db)


![ndqp](https://github.com/user-attachments/assets/ce796c48-a639-4b61-a68e-a96b5e5dce44)

