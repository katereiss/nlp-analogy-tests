**Project Proposal**

This project idea is inspired by: [Fair Is Better than Sensational: Man Is to Doctor as Woman Is to Doctor](https://direct.mit.edu/coli/article/46/2/487/93368/Fair-Is-Better-than-Sensational-Man-Is-to-Doctor) and [Large language models associate Muslims with violence](https://www.nature.com/articles/s42256-021-00359-2?proof=t).

The goal of this project is to compare the performance of NLP models trained on datasets from two different time periods using analogy tests for word embeddings. 

Wikipedia is used because it is a large collection of articles with available recent dumps (March 2022) as well as an archive from 2006. This will allow for sufficient depth while modeling, and the sixteen-year difference between the two may reflect differences in model performance.

Analogy tests are excellent metrics for how well a model can predict meaning of words. Words are represented as vectors, and the model calculates the cosine similarity between two words in an analogy to find the correct answer.

This visualization from Brian Spiering’s Data Ethics course provides an excellent representation of how analogy tests are solved.

<img width="597" alt="Screen Shot 2022-03-02 at 3 02 02 PM" src="https://user-images.githubusercontent.com/84412675/156464296-67574342-3956-4b78-9fcb-d04855b935af.png">

Also from Brian Spiering's Data Ethics course, an example of what an analogy test looks like is as follows.
<img width="991" alt="Screen Shot 2022-03-02 at 2 52 27 PM" src="https://user-images.githubusercontent.com/84412675/156464492-87ed3449-6bbf-41ab-96ee-4dbff24bee02.png">

Algorithms used will be unsupervised learning models including dimensionality reduction/topic modeling. Python libraries used will be pandas and scikit-learn for data cleaning and modeling, and possibly spaCy, gensim, or NLTK as needed.

An MVP would include results of many analogy tests for the models from both the 2006 and 2022 Wikipedia dumps. Further work would include improving the models to assess for and reduce biases in the analogy test answers.
