# Covid-19-prediciton

We are exploring images of chests of patients to detect the presence of covid-19.
Since COVID-19 attacks the epithelial cells that line our respiratory tract, we can use
X-rays to analyze the health of a patient’s lungs.

Link for the dataset:https://drive.google.com/open?id=1bIFGTSfrJgHWmh8_LUqsUVhW8ZWIdar3

For this purpose we are building our model on Google Colab to give us the necessary computation power and easy access to all the required libraries.

Following are the step-by-step procedure of training our model:

1:Importing data-sets from google drive

2.Extracting the images from the datasets and resizing them.

3.Converting the images into matrices with the help of open CV and normalizing the pixel-intensities to 255.

4.Extracting the labels of the images and converting them to one-hot-encoded-vectors.

5.Splitting data randomly into 75% training and 25% testing data.

6.Building A VGG-neural network architecture, a well known deep-convolutional-neural network which performs well on image datasets.
More about VGG-architecture can be found in this link:https://www.quora.com/What-is-the-VGG-neural-network

7.Using adam's optimizer algorithm to reduce the loss of our cost function.

8.Predicting the labels our our test-data after the model  is trained.

9.Creating the confusion-matrix, analyzing the accuracy,precison,f1-score and other measures and plotting the training loss(and accuracy) against the testing loss(and testing accuracy).

10.We were able to achieve a good 92% accuracy on the test set.




