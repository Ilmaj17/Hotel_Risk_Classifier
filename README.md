# Hotel_Risk_Classifier
Kaggle Link: https://www.kaggle.com/datasets/akshayramakrishnan28/hotel-risk-classification-dataset
I have build a data pipeline with two transformers and a final estimator.
The first transformer is to remove the 'content' column, which would be unnecessary in model prediction.
The second transformer is to convert the categorical 'tranlated_content' to numerical values. 
I have used LabelEncoder for this. Because OneHotEncoding may create a curse of dimensionality as the 'translated_column' has over 400 different values. Frequency encoding may result in ambiguity for those rows that may have same frequency.
Then finally I have choosed the DecisionTreeEstimator for model prediction which is a random pick, 
