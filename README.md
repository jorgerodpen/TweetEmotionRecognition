# Tweet Emotion sRecognition
 
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

===== **Instructions to run the code** =====
In the command line:
1. Extract all the files from the zip file
2. Change directory (cd) to the extracted folder
3. Create a virtual environment

python3 -m venv venv_name
source env/bin/activate

4. Install the required libraries from the requirements.txt file

pip install -r requirements.txt 

5. Open the testing jupyter notebook and run the code to see the outputs

jupyter notebook Model_Testing.ipynb