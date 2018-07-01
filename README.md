# Movie Review Sentiment with CNNs

We try to predict sentiment in movie reviews from the imbd dataset using CNN model. The first model includes a simple CNN with a embedding layer. 
The second model incldes a simple CNN model with pretrained model with GloVE word embeddings that are trainable and the final model incldes a vgg style model with pre-trained GloVe vector.
Ironically  a simple CNN model with a pre-trained word embedding (GloVe) does better than a complex CNN model .

Also as the dataset is small the network quickly overfits as is evident from accuracy 
train : 98-100% , 98% for larger model and 100% for smaller model with GloVe embeddings.However the test accuracy is around 87%. Showing that the model overfits the training data. The solution to this problem is to use a larger dataset and use of different drop outs or regularizers. 
