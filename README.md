# GS-Quantify-2019
The problem is identified as a text clustering task.
Dataset contains logs occurring with a certain pattern, leading to the formation of clusters

### Data cleaning steps - 
Lower casing, Punctuation removal, Stopwords removal, Rare words removal, Tokenization, Lemmatization. NLTK & TextBlob functions were used for cleaning.

### Text Transformation - 
Experimented following transformation methods
1. TF-IDF Vectorization - [here](https://github.com/pranavpawar3/GS-Quantify-2019/blob/master/Final_Code_pretrained.ipynb)
2. Word2Vec Transformation (Pretrained) - [here](https://github.com/pranavpawar3/GS-Quantify-2019/blob/master/Final_Code_transfer_pretrained.ipynb)
3. Word2Vec Using Transfer Learning Final - [here](https://github.com/pranavpawar3/GS-Quantify-2019/blob/master/Final_Code_transfer_learning.ipynb)

#### To download the Google News pretrained embeddings - [click here](https://drive.google.com/file/d/0B7XkCwpI5KDYNlNUTTlSS21pQmM/edit)

### Models used - 
1. K-Means
2. DBSCAN (Highest performing). Because of competition rules, no. of clusters can vary only between [5,20], and as DBSCAN was choosing more than 20 clusters as optimal, it was dropped from final model. 
3. Gaussian Mixture Models

### Dependencies - 
1. Pandas - 0.25.2
2. Numpy - 1.17.3
3. Matplotlib - 3.1.1
4. Sklearn - 0.21.3
5. NLTK - 3.4.5
6. Gensim - 3.8.1
7. logging

### Final Rank - 1st (Onsite finals at GS Office)
