'The dataset contains transactions made by credit cards in September 2013 by European cardholders.
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. 
The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues, 
we cannot provide the original features and more background information about the data. Features V1, V2, … V28 are the principal components obtained with PCA, 
the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and 
the first transaction in the dataset. The feature 'Amount' is the transaction Amount, 
this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.'

there is no much EDA since the data has hidden column names.

we used resampling techniques to overcome the challenges of unbalanced Class of data.

different types of classification model was used to come up with the model that best predicts whether a transaction is a fraud or not. 

RandomForestClassifier became our model of choice with the highest accuracy score.

during hypertuning of our model, i drastically reduced the size of our dataset because of the large computing power needed by the server. I even tried using google colab's GPUs
but the result was the same, took days to run it.
