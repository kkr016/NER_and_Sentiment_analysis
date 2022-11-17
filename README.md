# NER_Using_Scispacy_(NLP)
Named Entity Extraction Using Scispacy package


Objective 1: Extracting and counting most frequent entities from the tweets.
Objective 2: Finding the sentiment/polarity of each author towards each of the entities.

technique and packages used: Natural Language Processing, Data Pre-processing, Sentiment Analysis, Named Entities Recognition, Spacy, Scispacy, Pandas, Numpy, visualization, etc.,

The Approach to achieve the solutions

-	To implement the approach for Objective 1 problem is no leaned toward Data Preprocessing. (Cleaning data and removing Unnecessary elements from it.) Useless elements: Emojis, URL links, and others.
-	Because I am using Scispacy package for the Named entity recognition, which is mainly packed for scientific entities. Such as Chemicals, Diseases, Drugs, and also for general entities.

Steps involved in solving the Objective 1 are:
•	Download and import necessary packages & Download the Scispacy and Spacy module for the corpus
•	Raw data analysis
•	Conversion of Raw data to Data frame
o	Data Pre-processing (Cleaning Tweets)
o	Finding text with URL and remove
o	Replacing punctuations with space
o	Word less than 2 character
o	make entire text lowercase
o	remove stop words
o	Lemmatization

•	Check and compare the Spacy, Scispacy large module, Scispacy – module BC5CDR
•	 Extracting Entities from the tweets with their frequency using Scispacy large module
•	Data Visualization
•	Solution of Objective 1 (done)

Objective 1:
Difficulties:
-	While using the NLP n-gram techniques to find the entities gives more no. of n-grams and gets lots of time. And also, we get Nouns phrases most of the time it is meaningless too, and treating it as an Entity is a waste.
Technique I used for:
-	So, I was moved to technique Named entity recognition which the extracts the features NER, POS tagging, dependency parsing, word vectors and more.

Reason Why I chose it
-	Since the data sets were related to the Scientific bio medical revies and tweets. 
-	Hence, Scispacy is the most relatable Corpus had in the scientific domain. There are many modules were available. Here, I am using General Scispacy Large module and Biomedical module which as only NER entity of “Chemical and Diseases”
-	And Scispacy Module Gives the entities as rich as others modules
Note:	The entire NER is performed under the Preprocessed Columns which gives the best results.
Shortcomings and How I approached
-	Here, I omitted the other languages such as Japanese, Chines, etc. This will reduce the sentiment of the particular tweets.
-	And, also, I didn’t use the Dependency parses in the sentences which also gives the more detail to the entities which is extracted.

Steps involved in solving the Objective 2 are:
•	Downloading sentiment analysis tool i.e., NLTK "vader_lexicon"
•	Test the analyzer with own sentence with all types
•	Create the new columns as “sentiment score “, “polarity” with respect to the sentiment score
•	Solution of Objective 2 (done)

Objective 2:
Technique I used for is “vader_lexicon” of SentimentIntensityAnalyzer
Reason Why I chose it
•	Since the data sets were mixed of URL, Emojis, Emoticons, #hastags, Caps, @mentions, other languages, Etc., 
•	Hence, vader_lexicon Do not need the tweets precleaned
•	Because, All the mentioned characters give the major role in the polarity score using vader_lexicon model.
Note:	The sentiment score is performed under the Non-Preprocessed Columns which gives the best results.


