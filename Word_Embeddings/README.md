## Introduction to Word Embedding and Word2Vec

Word embedding is one of the most popular representation of document vocabulary. 
It is capable of capturing context of a word in a document, semantic and syntactic similarity, relation with other words, etc.
What are word embeddings exactly? Loosely speaking, they are vector representations of a particular word. 

Our objective is to have words with similar context occupy close spatial positions. 
Mathematically, the cosine of the angle between such vectors should be close to 1, i.e. angle close to 0.
Here comes the idea of generating distributed representations. Intuitively, we introduce some dependence of one word on the other words. 
The words in context of this word would get a greater share of this dependence. 
In one hot encoding representations, all the words are independent of each other, as mentioned earlier.

### How does Word2Vec work?
Word2Vec is a method to construct such an embedding. It can be obtained using two methods (both involving Neural Networks): Skip Gram and Common Bag Of Words (CBOW)
In the CBOW model, the distributed representations of context (or surrounding words) are combined to predict the word in the middle. While in the Skip-gram model, the distributed representation of the input word is used to predict the context.

### Glove - module for GloVe word vectorization (NumPy implementation)
GloVe is an unsupervised learning algorithm for obtaining vector representations for words. Training is performed on aggregated global word-word co-occurrence statistics from a corpus, and the resulting representations showcase interesting linear substructures of the word vector space.
