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



