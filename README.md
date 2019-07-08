# A Two-layer, Noise tolerant Auto Resonance Network for Image Recongition in MNIST database
Auto Resonance Network (ARN) is a new type of Artificial Neural Network.  It works as a generic data classifier. These networks were originally introduced for use in Robotic applications.  However, the use of these networks for other applications was not explored.  In this work, we present a two-layer ARN for image recognition in MNIST database.  
ARN has tunable nodes which adjust themselves to cover a certain range of inputs depending on the values of resonance control parameter (rho) and a threshold (T).
Theoretical background to estimate these parameters is made available online through our research papers.  
With tunable characterstics of ARN nodes, it is possible to achieve a recognition accuracy of 93% while using very few training samples as 50 images per digit (a total of 500 iamges).  This is achieved with rho=2.42, T=0.95 (layer 1) and T=0.9375 (layer 2).
The sample code to train ARN with 50x10 image samples is given. It can be easily modified to train more number of images.

The dataset was taken from publically available MNIST database. The database has 60,000 image samples for training and 10,000 image samples for test.
We have sorted the 60,000 images samples digit wise (0, 1, ...9) and taken only first 50 images of each digit, making a total of 500 image samples.  These are then used for training.
The original database has images in unicode form, we have converted them into pixel values to be between 0 to 255 and then normalized to be between 0 and 1.
