# Clustering Word Embeddings to Analyze Semantic Differences between Wikipedia and Twitter

**Introduction**

Inspired by the papers [Fair Is Better than Sensational: Man Is to Doctor as Woman Is to Doctor](https://direct.mit.edu/coli/article/46/2/487/93368/Fair-Is-Better-than-Sensational-Man-Is-to-Doctor) and [Large language models associate Muslims with violence](https://www.nature.com/articles/s42256-021-00359-2?proof=t), this project aims to answer the question: how do word embeddings differ by training them on text from different sources?

Word embeddings are representations of words as vectors, and words closer to one another have similar meaning or usage. Word embeddings are therefore an excellent tool for analyzing semantics of words. If vectors representing the same word are far from one another, this may be an indicator of this word having different meaning or usage between the two training corpora.

I was interested in finding out how an unsupervised clustering algorithm would cluster the data from both corpora, and if human biases would be apparent in one or both corpora. 

**Design and Data**

The two pre-trained models I used can be found  on the Gensim libary. One is from a 2014 Wikipedia dump containing 5.6 billion tokens and 400,000 words represented as 200-dimensional vectors, and the other is a collection of 2 billion tweets containing 27 billion tokens and 1.2 million words represented as 200-dimensional vectors. 

**Algorithms**

I used Principal Component Analysis (PCA) in order to reduce the dimensions from 200 to 125 and 100. 

The initial clustering model was a K-means clustering with 10 clusters for the Wikipedia embeddings and 20 clusters for the Twitter embeddings, based on inertia plots for both. 

I chose DBSCAN for an improved clustering algorithm, as cosine similarity was a more appropriate distance metric for these high-dimensional vectors than euclidean distance. 

**Tools**

- Gensim for data acquisition
- Pandas and Numpy for analysis
- Seaborn for visualization
- Scipy for distance calculations
- Scikit-learn for modeling

**Communication**

Presentation slides are attached to this repo.
