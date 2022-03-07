**MVP**

This project aims to answer the question: how do word semantics differ between models trained on text from different sources?

Word embeddings represent words as vectors, and words closer to one another have similar meaning or usage. 

In order to test this, I found two pre-trained models on Gensim: 2014 Wikipedia containing 5.6 billion tokens and 400,000 words represented as 200-dimensional vectors, and 2 billion tweets containing 27 billion tokens and 1.2 million words represented as 200-dimensional vectors. In this project, I will be clustering these word embeddings in order to find differences between word semantics in these models from different sources. 

My goal for this project is to depict how the initial data source we choose may influence the meanings of words in our model, in our results, and in our applications of NLP products. 

The initial clustering model is a K-means clustering of the Wikipedia model’s vocabulary with K = 10. 
<img width="529" alt="Screen Shot 2022-03-07 at 1 46 31 PM" src="https://user-images.githubusercontent.com/84412675/157123924-bc8b7cd3-0dd5-48ce-83b6-8e07ec6cd5b3.png">
<img width="518" alt="Screen Shot 2022-03-07 at 12 44 14 PM" src="https://user-images.githubusercontent.com/84412675/157124002-136be42c-a779-43af-81a4-40c562a4239e.png">


Additions will be repeating this clustering for the Twitter model’s vocabulary, exploring different clustering models and tuning hyperparameters, and appropriately visualizing the differences in the clusters from the two models. 

Other potential additions are removing stop words and punctuation from the vocabularies.
