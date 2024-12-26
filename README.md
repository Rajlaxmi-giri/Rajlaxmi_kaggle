Exploratory Data Analysis(EDA)

Data Loading: The dataset is loaded into the notebook using pandas and prepared for analysis
Summary Statistics: We compute basic statistics such as mean, median, standard deviation, and other descriptive measures to get an overview of the dataset.
Data Cleaning: Identifying missing values, duplicates, null value then count the no.value_counts
about text no.of character,no.of words & no.sentence .
finally display the polt about count.

Text Preprocessing

transforming raw data into format that is easier to understand and process by algorithms. It involves:
Lowercasing- convert all text to lowercase e.g. "Hello"->"hello"
Tokenization- split the text into smaller units such as words. e.g. "I am a programmer"->["I","am","a","programmer"]
Removing Punctuation- Eliminate special characters and punctuation e.g. "hello!"->"hello"
Removing stop words- Eliminate common words like "and","the","in",etc that don't add much meaning
Stemming- reduce words to their root form e.g. "running"->"run" OR Lemmatization- converts word to their base form with meaning.


Word visualization

1.In our model use word counts to understand disaster and not disaster.This helps us identify patterns.
2.Words commonly used in disaster-related tweets like:- help,flood,emergency,earthquake,victims,fire.
3.Words commonly used in Non-disaster related tweets like:- weekend,party,family,happy,movie,dinner.
4.After counting, we plot bar chart the results to see the distribution of words in each category.

Feature engineering

Feature engineering is the process of converting text data into a numerical format.
1.In our model use Count Vectorization ,TF-IDF and Word2Vec is a more advanced technique.
2.Count Vectorization :- It counts how many times each word. 
    For example:  'I like cats',' I like dogs' -->the word 'like' appears twice, so its count is 2.
3.TF-IDF :- improves on Count Vectorization by not just counting the words but also assigning weights.
    For example: 'the' or 'and,' are less useful and get lower weights.
4.Word2Vec:- creates 'word embeddings' way to capture the meaning of words and their relationships to one another. It uses a neural network to understand the context in which words appear.

model building

In this project, i am using bow and tf-idf we compared the performance of four machine learning algorithms—Logistic Regression,
Naive Bayes, Random Forest, and Support Vector Machine (SVM)—on the given dataset.The primary evaluation metric used was accuracy.
Among the models evaluated, Logistic Regression achieved the highest accuracy of 81.29%, 
making it the best-performing model for this dataset. Naive Bayes closely followed with 80.76%, while Random Forest achieved 77.87%. 
The SVM model performed the worst with an accuracy of 59.03%, likely due to insufficient tuning or mismatched assumptions.
Model Accuracies:
Logistic Regression: 0.8129
Naive Bayes: 0.8076
Random Forest: 0.7787
svm : 0.5903

Using Word2Vec :
Model Accuracies:
Logistic Regression: 0.68
Random Forest: 0.69
svm : 0.42

Using Word2Vec + TF-IDF  :
Model Accuracies:
Logistic Regression: 0.75
Random Forest: 0.72
svm : 0.74

Conclusion 

"Our results show that Logistic Regression outperforms other algorithms in terms of accuracy, achieving the highest accuracy at 81.29%. Therefore, Logistic Regression is the best model for this dataset based on accuracy."


