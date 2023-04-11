# Image_captioning using LSTM and Transformer decoders

**Using LSTM decoder

* Used stochastic updates instead of batch updates i.e., one image at a time is used for updating the network.

* VGG network is used as feature extractor (512 dimensional feature vector for every image)


**Using Transformer decoder

* Used 4 transformer blocks, 8 heads, hidden size 512, batch size 128, Adagrad optimizer, gelu activation.

* IceptionNet is used as feature extractor (6x6x2048 reshaped to 36x2048 dimensional features for every image)

* You can see difference in generated captions after training for 500 epochs, 1000, 1500, 2000 epochs and at the end captions for unseen data. 

**Using Vision Transformer architecture as encoder and trnasformer as decoder

* Transformer architecture is same as above for both encoder, decoder. 

* Encoder is trained from scratch, so since there is no pretraining on images, it lacks generalization capability and overfits (generating exact caption as in the training set, generating irrelavent caption for test image). 

* You can see generated captions after every 300 epochs of training.




** Data set used is Flickr8k, first 8000 images are used for training, remaining 90 images are used for validating in all the 3 architectures.
