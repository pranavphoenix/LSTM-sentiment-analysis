# LSTM-sentiment-analysis
## Using LSTM for sentiment analysis of IMDB movie reviews and using GloVe Embeddings for analogy tasks
### Analogy
- Prince – Boy + Girl = Princess
- King – Man + Woman = Queen
- Chinese – China + India = Indian
- Larger – Large + small = Smaller
###### We used different dimensional glove embeddings to create the analogies and compared the norm of the resultant vector with the actual result of the analogy. To get the closest matching word vector, we used the most_similar function from genism which finds the closest vector in terms of cosine similarity

### Sentiment Analysis using LSTM
###### We are using Keras libraries to build the LSTM network for sentiment classification.
###### Dataset: IMBD movie reviews (IMDB movie review sentiment classification dataset, n.d.)
###### We have chosen reviews of maximum length up to 500 words
###### Train data = 42882 reviews
###### Vocabulary = 40000 words
###### Train validation split = 0.8
###### Test data = 3065 reviews
###### Padding was done
###### Input => embedding layer=>LSTM=>sigmoid
