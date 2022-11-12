Summary: Sentiment analysis of apparel E-commerce text reviews to predict whether items will trend

Dataset: 23,486 reviews from "Womens Clothing E-Commerce Reviews.csv"

Description:
- Filter Clothing IDs with at least 5 reviews
- Remove punctuations and change words in review texts to lowercase
- Remove stopwords based on NLTK's stopword corpus
- Tokenize, lemmatize and apply POS-tagging
- Apply Tf-Idf vectorization
- Conduct hyperparameter tuning for Logistic Regression, Support Vector Classifier, Random Forest and Multinomial Naive Bayes
- Apply Text Embedding layer for Deep Learning models
- Determine optimal thresholds from [0.5, 0.6, 0.7, 0.8, 0.9] that maximizes F-beta score (beta=0.5)
- Apply optimal thresholds on test predictions for each model
- Compare accuracy and F-beta scores

Results:
- Logistic Regression (83.1%, 0.325)
- Support Vector Classifier (86.3%, 0.038)
- Random Forest Classifier (86.2%, 0.268)
- Multinomial Naive Bayes (86.1%, 0.199)
- Convolutional1D Neural Network with Tf-Idf embedding layer (86.3%, 0)
- Neural Network with 2 Dense layers and Tensorflow Hub's Universal Sentence Encoder embedding layer (86.5%, 0.332)