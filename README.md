# Character-Recognition_-A-Z-0-9-
Implemented a machine learning model using tensorflow , Keras and NN(neural networks) in python.


In the jupyter notebook created a model along with gui using tkinter.


Dataset for digit is imported from keras and dataset for character is downloaded from https://www.kaggle.com/datasets/sachinpatel21/az-handwritten-alphabets-in-csv-format


DIGIT dataset - rows:70,000          columns:784


ALPHABETS dataset - rows:370000      columns:784


for the detection of character , 
first we resize and reshape(28*28) the input image using opencv.
how it detects?
for detection it reads value from each cell of the image matrix as 0-255 (0 for black and 255 for white).
then this 28*28=784 values are compared with the dataset and gives the most accurate output.


NOTE:
we divided the pixel-values by 255 for better accuracy than whole numbers(0-255). so 1 is for white and 0 is for black.


for the clash of first charcter(A) and first-digit(0) we have created a dictionary.



dictionary = ['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z','0','1','2','3','4','5','6','7','8','9']
