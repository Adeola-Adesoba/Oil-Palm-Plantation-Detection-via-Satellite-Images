# Oil-Palm-Plantation-Detection-via-Satellite-Images
This notebook provides image classification work on satellite images using transfer learning approach
This notebook provides a fine tuning mechanism when using pre-trained network for binary image classification.
-----------
A pre-trained model is used i.e. VGG19 network and the weights is initialized using the weights trained on imagenet database.
To obtain the final model tailored to the dataset used in this work, the network is trained twice.

In the first training, the convolutional layers of VGG19 is freezed (forcing the network to use the weights trained on imagenet database).

In the second training, the network is initialized with the weights obtained from the first training and further fine tuned using stochastic gradient descent optimizer

In conclusion, the final model was able to predict the prsence of oilpalms with an accuracy of 99.7%.
