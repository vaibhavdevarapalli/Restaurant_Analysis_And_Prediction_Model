# Restaurant Reviews Sentiment Analysis
This project involves building a sentiment analysis model for restaurant reviews using the Bag-of-Words (BoW) model and Naive Bayes classification. The project includes data preprocessing, model training, and predicting sentiments on new data.

## Datasets
### Historic Dataset (a1_RestaurantReviews_HistoricDump.tsv):
- Contains 900 restaurant reviews with labeled sentiments (0 for negative, 1 for positive).
- Data Format: Tab-separated values with two columns: Review (text) and Liked (label).

### Fresh Dataset (a2_RestaurantReviews_FreshDump.tsv):
- Contains 100 new restaurant reviews without sentiment labels.
- Used for predicting sentiments with the trained model.

## Files and Models
### Preprocessed Data and Model:
- c1_BoW_Sentiment_Model.pkl: BoW dictionary used for feature extraction.
- c2_Classifier_Sentiment_Model: Trained Naive Bayes classifier.

### Predicted Results:
- c3_Predicted_Sentiments_Fresh_Dump.tsv: Predicted sentiments for the fresh dataset.

## Workflow

### Historic Data Processing

#### - Dataset: a1_RestaurantReviews_HistoricDump.tsv (900 reviews)
#### - Preprocessing: Cleaned and tokenized text data, removed stopwords, and applied stemming.
#### - Feature Extraction: Created BoW dictionary with 1420 features.
#### - Model Training: Trained a Gaussian Naive Bayes classifier on the processed data.
#### - Model Performance: Achieved an accuracy of 72.78% on the test set.

### Predicting Sentiments on New Data

#### - Dataset: a2_RestaurantReviews_FreshDump.tsv (100 reviews)
#### - Preprocessing: Applied the same cleaning and tokenization steps as historic data.
#### - Prediction: Loaded the pre-trained BoW model and classifier to predict sentiments on the new dataset.

## Dependencies
- Python 3.x
### Required Libraries:
- numpy
- pandas
- scikit-learn
- nltk
  
## Results
- The model correctly predicts positive and negative sentiments with an accuracy of 72.78% on the test set.
- Predictions for the fresh dataset are saved in c3_Predicted_Sentiments_Fresh_Dump.tsv.

  

