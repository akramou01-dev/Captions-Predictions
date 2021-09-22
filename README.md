# Captions-Predictions

In this notebook we use a pre trained ResNet50 model from Keras, we delete it's last layer so that we have a vector of 2048 for the output we give this vector to another model which contain Danse and RepeatVector Layers.
We creat also another NLP Model to predict the words of the captions based on the captions in the Dataset  (Flickr_Data). The NLP model contains an Embedding layer as an input , a LSTM and a TimeDistributed layers.
We concatenate them and pass the result of the concatenation to another model which contains 3 LSM Layers and an Activation fonction "Softmax".
After training the model we had an accuracy of 88.76% on the training data .
Enjoy Reading and contacte me if you have a questions. 
