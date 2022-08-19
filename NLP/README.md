Summary:
Sentiment analysis to classify texts from medical journal abstracts into the following categories (objective, background, method, results, conclusion)

Dataset:
20,000 lines of text from https://github.com/Franck-Dernoncourt/pubmed-rct

Description:
- Preprocess txt file into dictionary with the following keys (target, text, line number, total number of lines)
- Encode the labels using OneHotEncoder and LabelEncoder
- Build and fit a non-Neural-Network Naive Bayes model as baseline
- Create dataset batches and use parallelisation to optimise flow
- Create a token-level TextVectorizer and Embedding layer to build a Convolutional 1D model (model 1)
- Use pretrained Embeddings from Tensorflow Hub's Universal Sentence Enocder to build model 2
- Create a character-level TextVectorizer and Embedding layer to build a Convolutional 1D model (model 3)
- Concatenate the token-level and character-level Embedding layer into a Hybrid layer to build model 4
- Create a positional Embedding layer and concatenate with the Hybrid Layer to build a Tribrid layer for model 5
- Compare the F1_scores across model 1 to 5

Results:
- Baseline 69.9%
- Token-level embedding 78.1%
- Pretrained token-level embedding 70.1%
- Character-level embedding 59.6%
- Hybrid embedding 73.1%
- Tribrid embedding 83.1%
