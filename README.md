# AutoEncoders

Auto Encoders are maily used for dimensionality reduction or in other words it is used to compress the data. 

It can be used to visualize the data in lower diamension.

Another important use of auto encoders is to find or reveal the hidden relationship between the features, that are not visible in the higher diamensionality.

Here I have created encoder units with Dense and Flatten layer. I have also created the decoder units with Dense and Reshape layer.

Important point to note in case of AutoEncoders are the number of neurons in the input layer and the output layer should be same.

We have started with 400 neurons and slowly reduced it to 25 in the encoder layout. In the second half (decoder section) the autoencoder will exapnd the neurons back to the number of neurons that we started with.

The internal hidden layer will learn the what features are important to produce the output at the final layer.

Here I have used loss function as "Sigmoid" since will be using "binary_crossentropy" during the model compiling part. 

Even though we have 0-9 images to predict, we will be comparing the input image with output image. That is why I have used "binary_crossentropy" as loss function.
