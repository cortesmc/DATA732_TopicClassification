# DATA732_TopicClassification

The objective on this project is to apply differents approches to make a semantic classification/Clustering to a data set of articles.  
The dataset comes from the study realized by Ph.D. candidate and engineer in Data Science Paul Mathieu.


# Pipeline of the study

0.TD_plotly: Introduction to Plotly and Dash uses in python.   
 
1.Dataframe_creation: The initial dataset "preprocess-topaz-data732" comes in a Json format. This NoteBook let's me generate pandas dataframes to utilize in the next parts of the study.   

2.1.kmeans_clustering:  First approach to clustering using a kmeans methode with a TF IDF methode of vectorization.    

2.2.LDA_Cluster: Second approach to make a semantic clustering of the articles using Latent Dirichlet Allocation(LDA) with CountVectorizer. This code uses as a guide this [kaggle publication](https://www.kaggle.com/code/hamditarek/topic-modeling-lsa-and-lda)   

3.1.LDA-CountVect_content_cluster: LDA + CountVectorizer with a different set of parametrization to compare the use LDA with differents inputs; CountVectorization in this case.    

3.2.LDA-TFIDF_content_cluster: LDA + TfidfVectorizer with a different set of parametrization to compare the use LDA with differents inputs; TfidfVectorizer in this case.   

4.bert_ZeroShotLabel: Approach of using a zero-draw classification model to assign labels to items. This approach was not developed due to the high process required to perform the calculations.
