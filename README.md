# text-summarization
Text Summarization is one of those applications of Natural Language Processing (NLP) that aid in generating precise and concise summary of big text while focusing on the sections that convey useful information, without loosing the overall meaning.
Text summarization aims to transform lengthy text into short versions, which would otherwise be an arduous task if done manually.

Approach used:
  Text Rank Algorithm: 
  There exists a very famous algorithm for this sort of Text Summarization i.e. TextRank.
  TextRank finds its roots associated with Google’s PageRank (by Larry Page) used for ranking webpages for online search results. But before unfolding TextRank, we must understand PageRank & the intuition behind it:
  PageRank assumes that the rank of a webpage W depends on the importance of a webpage suggested by other web pages in terms of links to the page i.e. if a webpage ‘X’ has a link to webpage ‘W’, ‘X’ contributes to the importance of ‘W’.

TextRank also uses the same logic as in PageRank but with some subtle changes:
  In place of web pages, we use sentences.
  Similarity between any two sentences is used as an equivalent to the web page transition probability.
  The similarity scores are stored in a square matrix, similar to the matrix M used for PageRank.
  The similarity matrix for index [A, B] is filled with similarity values between sentences A & B rather than 1/total_links from Page B to A which can be calculated using either cosine distance, maximum common words, etc..

![image](https://github.com/divanshu-walia/text-summarization/assets/150337265/426860b5-3cc3-432c-8c84-60c18d341a00)

Libraries Used: Pandas, NumPy, Contractions, Re, NLTK (sent_tokenize, stopwords), Sklearn (cosine similarity), Networkx.

![image](https://github.com/divanshu-walia/text-summarization/assets/150337265/ab2fe450-c002-4fb9-b0a6-5d2eb660bb7d)


