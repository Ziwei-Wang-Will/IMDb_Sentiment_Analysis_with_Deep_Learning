# IMDb_Sentiment_Analysis_with_Deep_Learning

<img src="https://github.com/will-zw-wang/IMDb_Sentiment_Analysis_Using_Deep_Learning/blob/master/images/IMDb_image.jpg" width="960" height="200">

[**Detailed Code and Plotting**](https://github.com/will-zw-wang/IMDb_Sentiment_Analysis_Using_Deep_Learning/blob/master/IMDb_Sentiment_Analysis_Using_Deep_Learning.ipynb)

## Project Objectives

- Our problem at hand is to classify movie reviews as positive or negative using the text of the review.

## Dataset description
- A widely-used dataset for this task is the [IMDB dataset](https://www.tensorflow.org/api_docs/python/tf/keras/datasets/imdb). 
  - It contains 50,000 movie reviews from IMDB, and preprocessed into 25,000 reviews for training and 25,000 reviews for testing, both sets are balanced.
  
## Analysis Structure
1. Basic preprocessing of NLP data
2. Built a model using FNN
3. Improvements to the model - dealt with overfitting
4. Model Comparison

## Analysis Details

### 1. Basic preprocessing of NLP data
- Tokenized words
- Created a dictionary that maps words to unique IDs
- Converted words to ID
- Padded/truncated sequences to unified lengths

### 2. Built a model using **FNN**
- Designed model structure
- Added layers
- Defined loss
- Defined optimizer
- Created a plot to clearly observe training progress
- Evaluated on test set

### 3. Improvements to the model - dealt with overfitting
- **Dropout**
- Built a recurrent model
  - **LSTM**
  - Improvements to a recurrent model
    - **Deep LSTMs**
    - **Bi-directional RNN**
    - Combined **deep LSTM** with **bi-directional RNN**
- **Pretrained embeddings**
  - Used the **GloVe embeddings** to initialize our embedding weights
- Mixture of the above 

### 4. Model Comparison
- <img src="https://github.com/will-zw-wang/IMDb_Sentiment_Analysis_Using_Deep_Learning/blob/master/images/Model_performance_comparison.png" width="500" height="240"> 
- Combining **pretrained embeddings**, **dropout** and **LSTM**, we improve the model performance slightly from 83% to 84, and **pretrained embeddings** makes greater contribution to this improvement than the others.
