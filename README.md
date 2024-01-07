# DATA732_TopicClassification

The objective on this project is to apply differents approches to make a semantic classification/Clustering to a data set of articles.  

The dataset comes from the study realized by Ph.D. candidate and engineer in Data Science Paul Mathieu.   

# Pipeline of the study

* 0.TD_plotly: Introduction to Plotly and Dash uses in python.   
 
* 1.Dataframe_creation: The initial dataset "preprocess-topaz-data732" comes in a Json format. This NoteBook let's me generate pandas dataframes to utilize in the next parts of the study.   

* 2.1.kmeans_clustering:  First approach to clustering using a kmeans methode with a TF IDF methode of vectorization.    

* 2.2.LDA_Cluster: Second approach to make a semantic clustering of the articles using Latent Dirichlet Allocation(LDA) with CountVectorizer. This code uses as a guide this [kaggle publication](https://www.kaggle.com/code/hamditarek/topic-modeling-lsa-and-lda)   

* 3.1.LDA-CountVect_content_cluster: LDA + CountVectorizer with a different set of parametrization to compare the use LDA with differents inputs; CountVectorization in this case.    

* 3.2.LDA-TFIDF_content_cluster: LDA + TfidfVectorizer with a different set of parametrization to compare the use LDA with differents inputs; TfidfVectorizer in this case.   

* 4.bert_ZeroShotLabel: Approach of using a zero-draw classification model to assign labels to items. This approach was not developed due to the high process required to perform the calculations.


# Use if the pipeline

In all the study i used two differents dataframes, both generated in [1.Dataframe_creation]. One of the dataframes has 965 articles and the other is the recopilation of all the sources of articles (with 36592 articles in total). Because t=of the high demand of capacity of process all of the notebook were developped with the small dataframe but they all work with the any quantity of articles if they have the correct format.

1. In order to use the pipeline, you need to add all the input Json files in the "preprocess-topaz-data732" file.
2. Then you can run all the notebooks in order of the names from 1.Dataframe_creation.
3. On each notebook you can choose which file use to make the sutdy on.
4. All the results can be saved by uncommenting the last lines of each notebook. 

# Results

All the important results are saved on .csv format in the file "results".
These files are used on the two tableau files with the names: Final_results_KmeansTfIdf.twb and Final_results_LDA_CntVect.twb.
All the explication and conclutions found in this study are presented and explained on the final report.