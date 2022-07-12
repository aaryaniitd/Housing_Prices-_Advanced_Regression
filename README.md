# Housing_Prices_Advanced_Regression
Code for the Advanced Regression - Housing Prices Kaggle competition.

#### Process:
1. I separated training data into int columns and object columns. The int columns were kept undisturbed but the object columns had to be converted to float or int datatype.
2. I used Hot Encoding on the 'object' type columns which had other than 'True/False' or 'Yes/No' values.
3. After converting all object type forms to int/float, I merged the dataset and filled the nan values with the mean of the column.
4. I then used SelectKBest from sklearn.feature_selection to find the contribution score of every column to the target column. The best 100 features were selected for model training. 
5. I used RandomForestRegressor from sklearn.ensemble for creating the model. The error score was 0.177 (competition best: 0.0, worst: 24.696).
