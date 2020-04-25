# Covid-19-prediciton

We are exploring X-ray images of chests of patients to detect the presence of covid-19.
Since COVID-19 attacks the epithelial cells that line our respiratory tract, we can use
X-rays to analyze the health of a patient’s lungs.

Link for the dataset:https://drive.google.com/open?id=1bIFGTSfrJgHWmh8_LUqsUVhW8ZWIdar3

For this purpose we are building our model on Google Colab to give us the necessary computation power and easy access to all the required libraries.

Following are the step-by-step procedure of training our model:

1:Importing data-sets from google drive

2.Extracting the images from the datasets and resizing them.

3.Converting the images into matrices with the help of open CV and normalizing the pixel-intensities to 255.

4.Extracting the labels of the images and converting them to one-hot-encoded-vectors.

Note:We are now working on created a CNN model for this dataset to train our model and get desired results.



