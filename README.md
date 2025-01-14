2018 Summer Research Project    
Research Group: Machine Learning for Data Science  at University Carlos III in Madrid, Spain     
PI: Jerónimo Arenas-García    

Topic Modeling Using a Dataset of BBC News Articles
---------------------------------------------------
The "bbc-dataset-201601-201607-time.tab" dataset that was used is available at the URL   
https://github.com/BBC-News-Labs/Text_Analytics/tree/master/data-from-Juicer  

The goal of the project was to create a visualization tool to provide insight into the distribution of relevant topics in a dataset of BBC news, with respect to geographic area. In order to do so, Natural Language Processing tools have been applied to carry out the following tasks:
- Preprocessing of 36,163 text documents using tokenization, stop word removal, stemming, and n-gram extraction
- Creation of topic models using Latent Dirichlet Allocation 
- Automatic annotation of topics   

In order to allow for an easier exploration of the results, a visualization tool has been developed, showing the distribution of topics across UK regions using Google Fusion Tables. This tool allows also the user to incorporate filters, so that specific topics or geographic regions can be better analyzed and compared.

Google Fusion Table Link:
https://www.google.com/fusiontables/DataSource?docid=1z216Q5u4paybZrqnNEq2xVKBLLcyu3urb21QShzp

Files 
-----
- create_BBCnews_table.py - created SQLite database for the news articles and read in dataset into a table
- preprocess_words.py - preprocess the words for each article in the table
- create_LDAmodel.ipynb - create the LDA model 
- create_Topic2Words.ipynb - create a csv file of each topic and top 10 associated words
- topic2word_proportions.ipynb - create a csv file of each document and the topic proportions
- find_top_topic.ipynb - find the top topic for each document
- update_newsdatabase.ipynb - update BBC news table with corrected tags
- fusiontable_data.ipynb - create separate uk table with the UK articles
