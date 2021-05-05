# Tweet Emotions Recognition
 
- Created two classifiers (an MLP and a SVM) for Tweet emotion detection: <code>anger</code>, <code>joy</code>, <code>sadness</code> and <code>optimism</code>. 
- Grid-searched the MLP and the SVM to look for the optimal hyper-parameters.
- Used random undersampling, random oversampling and SMOTE to handle data imbalance. 
- The best SVM model had an F1 weighted score of 0.665 and was trained with the original data
- The best MLP model had an F1 weighted score of 0.601 and was trained with SMOTE applied to the training data. 

## Packages
**Python Version:** 3.8.3

**Packages used:** pyspark, pandas, numpy, scikit-larn, imblearn, matplotlib, seaborn, pytroch, skorch

**Requirements:** <code>pip install -r requirements.txt</code>

## Source of data
The original data was downloaded from [tweeteval](https://github.com/cardiffnlp/tweeteval) repo, from the folder *Emotion Recognition*. 

## Data cleaning
- Merged all the datasets and split them in 75% training set and 25% test set. 
- Parsed the Tweets with a bag of n-grams approach. 
	- The best SVM model was trained with 1-grams and with stopwords removed
	- The best MLP model was trained with 1-grams and with stopwords removed


## Specifications 
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