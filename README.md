# Image_captioning using LSTM and Transformer decoders

**Using LSTM decoder

Used stochastic updates instead of batch updates i.e., one image at a time is used for updating the network.


**Using Transformer decoder

Used 4 transformer blocks, hidden size 512, batch size 128, Adagrad optimizer, gelu activation.

You can see difference in generated captions after training for 500 epochs, 1000, 1500, 2000 epochs and at the end captions for unseen data. 

Data set used is Flickr8k
