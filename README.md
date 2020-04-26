# Covid-19-prediction

Coronavirus disease 2019 (COVID-19) is a highly infectious disease caused by severe acute respiratory syndrome coronavirus 2. The disease first originated in December 2019 from Wuhan, China and since then it has spread globally across the world affecting more than 200 countries. The impact is such that the World Health Organization(WHO) has declared the ongoing pandemic of COVID-19 a Public Health Emergency of International Concern.

![plot3](https://user-images.githubusercontent.com/44751602/80305404-08e3f980-87da-11ea-907f-956548efe046.png)

Though research suggests that social distancing can significantly reduce the spread and flatten the curve as shown, but is that sustainable? 

![plot5](https://user-images.githubusercontent.com/44751602/80305443-52ccdf80-87da-11ea-8e70-91ba16075120.png)

Fast and accurate diagnostic methods are urgently needed to combat the disease. In a very recent paper ‘A deep learning algorithm using CT images to screen for Corona Virus Disease (COVID-19)’ published by Shuai Wang et. al they have used Deep Learning in extracting COVID-19’s graphical features from Computerized Tomography (CT) scans (images) in order to provide a clinical diagnosis ahead of the pathogenic test, thus saving critical time for disease control.

The study used transfer learning with an Inception Convolutional Neural Network (CNN) on 1,119 CT scans. The internal and external validation accuracy of the model was recorded at 89.5% and 79.3%, respectively.

Link for the paper:https://www.medrxiv.org/content/10.1101/2020.02.14.20023028v4

In our study,we are not dealing with CT scan images but exploring images of chests of patients to detect the presence of covid-19.
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




