# Tweet Emotions Recognition

- Downloaded the original Tweets from [tweeteval](https://github.com/cardiffnlp/tweeteval) repo. 
- Cleaned the original files to create a train and test sets (75% and 25% respectively). 
- Grid-searched a MLP and a SVM to look for the optimal hyper-parameters.
- Used random undersampling, random oversampling and SMOTE to handle data imbalance. 
- The best SVM model had an F1 weighted score of 0.665 and was trained with the original data
- The best MLP model had an F1 weighted score of 0.601 and was trained with SMOTE applied to the training data. 

===== **Jupyter Notebooks** =====

All jupyter notebooks are available as ipynb and html files

- Cleaning: Contains the cleaning process of the original data to build the training and test sets
- SVM_tuning: Contains the grid-searches for the SVM parameters with the different approaches to handle data imbalance.
- MLP_tuning: Contains the grid-searches for the MLP parameters with the different approaches to handle data imbalance. 
- results_discussion: The results for the grid-searches are analysed and the best models are saved. 
- Model_Testing: Contains all the necessary code to run and test the two best models. 

===== **Folders** =====

- emotion: Contains the original txt files with the source data
- Data: Contains the CSV files with the final data
- Grid-Search: Contains the CSV files with the results for the grid-searches.
- Models: Contains the files of the two best models.