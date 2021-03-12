# Pattern Recognition Using Eigen Digits
## Project Overview
* MNIST digit dataset is used
* Eigen values and eigen vectors are calculated
* Reconstructed Handwritten digits
* Classification using Linear Regression
* Classification using Polynomial Regression
* Programming Language - MATLAB
__________________________________________________________
## Environment Setup
* MATLAB
________________________________________________________________
## Dataset
* [MNIST Handwritten Digit Dataset](http://yann.lecun.com/exdb/mnist/)
____________________________________________________________________
## Calculation of Eigen Value and Eigen Vectors
* Centered the data
* Calculated Covariance matrix

### Eigen - Digits Images
![image](https://user-images.githubusercontent.com/50255936/110647209-982bad00-81f2-11eb-8c20-c33cea625af0.png)
___________________________________________________________________________
## Image Reconstruction
* Original Test Images are projected into the subspace spanned by the top 30 eigenvectors by usign the following equation
![image](https://user-images.githubusercontent.com/50255936/110647720-0a9c8d00-81f3-11eb-802e-e4c63ea7baaf.png)
* Reconstructed data point is obtained by the following equation:
![image](https://user-images.githubusercontent.com/50255936/110647986-4d5e6500-81f3-11eb-915d-7bc4312a955e.png)

### Original Images (first row) vs Reconstructed Test Images (second row)
![image](https://user-images.githubusercontent.com/50255936/110648154-6e26ba80-81f3-11eb-825c-9f5b729d587d.png)
______________________________________________________________________________________________
## Classification of Digit using Eigen - Digits

* Mean of training digits is subtracted from both of the train images and test images (Centering)
* Subtracted Data points are projected into the subspae spanned by the top 30 eigen vectors

## Using Linear Regression

* Weight vector is calculated first

![image](https://user-images.githubusercontent.com/50255936/110659283-6704aa00-81fd-11eb-896c-e1d7578dcb76.png)

![image](https://user-images.githubusercontent.com/50255936/110659467-91566780-81fd-11eb-84b2-39f0553b1b2b.png)

* Predicted values are calculated as follows:
![image](https://user-images.githubusercontent.com/50255936/110656381-dcbb4680-81fa-11eb-9c11-9517ee0409c2.png)

### Block Diagram of the implementation of Linear Regression Model
![image](https://user-images.githubusercontent.com/50255936/110656495-f65c8e00-81fa-11eb-910d-33442eb8a81d.png)

### Classification Accuracy
![image](https://user-images.githubusercontent.com/50255936/110656583-0b392180-81fb-11eb-9202-865ad80c0993.png)

### Confusion Matrix
![image](https://user-images.githubusercontent.com/50255936/110656702-260b9600-81fb-11eb-8d0d-39f16b97ff4d.png)

## Using Polynomial Regression
* Second order polynomial is used
* Second order polynomial matrix for both train images and test images is setup according to the following equation:

![image](https://user-images.githubusercontent.com/50255936/110657286-adf1a000-81fb-11eb-830c-cbcb531eda04.png)

* Weight vector is calculated as follows:

![image](https://user-images.githubusercontent.com/50255936/110659679-c06cd900-81fd-11eb-9639-8a0b432df364.png)

![image](https://user-images.githubusercontent.com/50255936/110659711-c8c51400-81fd-11eb-9ae9-c7e5b6f30874.png)

* Predicted values are calculated as follows:
![image](https://user-images.githubusercontent.com/50255936/110657461-ce215f00-81fb-11eb-959e-16f36984b8f6.png)

### Block Diagram of the implementation of Polynomial Regression
![image](https://user-images.githubusercontent.com/50255936/110657588-e8f3d380-81fb-11eb-8961-8f68c942cd16.png)

### Classification Accuracy
![image](https://user-images.githubusercontent.com/50255936/110657647-f8731c80-81fb-11eb-9e42-15e5a5aa91ba.png)

### Confusion Matrix
![image](https://user-images.githubusercontent.com/50255936/110657693-0163ee00-81fc-11eb-9fe6-bf96200e4ea6.png)

## Training Vs Testing Accuracy for Linear Regression over Number of EigenVectors (Features)
![image](https://user-images.githubusercontent.com/50255936/110657956-3c662180-81fc-11eb-87f0-cd80757d7ee4.png)

## Training Vs Testing Accuracy for Polynomial Regression over Number of EigenVectors (Features)
![image](https://user-images.githubusercontent.com/50255936/110658649-d29a4780-81fc-11eb-9416-ea51299eacf2.png)





