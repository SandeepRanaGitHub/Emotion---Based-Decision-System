# Emotion Understanding--Decision System
<br>
This project builds an intelligent system that analyzes user inputs (journal text + contextual features) to predict emotional state, intensity, and recommend actions.
<br>
###Approach
<br>
Text preprocessing using NLTK (tokenization, stopword removal, lemmatization)
<br>
TF-IDF vectorization (unigram + bigram)
<br>
Feature combination with numerical + categorical data
<br>
Dimensionality reduction using TruncatedSVD
<br>
Emotional State → RandomForestClassifier
<br>
Intensity → RandomForestRegressor
<br>
### Feature Engineering
<br>
Text → TF-IDF (5000 features)
<br>
Categorical → One-hot encoding
<br>
Numerical → Standard scaling
<br>
Combined using sparse matrix stacking
<br>
Reduced to 100 dimensions using SVD
<br>
### Model Choice
<br>
Random Forest for robustness and interpretability
<br>
Handles mixed data types well
<br>
Works effectively with small-medium datasets
<br>
### How to Run
<br>
Train models using training dataset
<br>
Run prediction pipeline on test dataset
<br>
Output saved as predictions.csv
