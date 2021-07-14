1. To design the pipeline for ML workflow, custom tranformers have been created for followingstages -data cleaning,tokenizing,stopword removal,filtering words of length <1 and tf-idf computation.
2.Data cleaning is used to remove punctuations, undefined chars, numerals, links from tweets.
3.Tokenizing creates tokens of the tweets, nltk’sword_tokenize()is used to create tokens.
4.Stopwords are removed , stopwords obtained from nltk’s corpus.
5.CustomFilter()transformer removes tokens of length less than 1.
6.Map-reduce paradigm used to compute tf-idf of tweets. Pipeline = Pipeline(stages=[cleaner, tokenizer, remover, final, tfidf])


