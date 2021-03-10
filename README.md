# Pattern Recognition Using Eigen Digits
## Project Overview
* MNIST digit dataset is used
* Eigen values and eigen vectors are calculated
* Reconstructed Handwritten digits
* Classification using Linear Regression
* Classification using Polynomial Regression
* MATLAB is used
__________________________________________________________
## Environment Setup
* MATLAB
________________________________________________________________
## Dataset
* [MNIST Handwritten Digit Dataset] (http://yann.lecun.com/exdb/mnist/)
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
![image](https://user-images.githubusercontent.com/50255936/110656289-c7deb300-81fa-11eb-9eb6-18d262eb0498.png)
* Predicted values are calculated as follows:
![image](https://user-images.githubusercontent.com/50255936/110656381-dcbb4680-81fa-11eb-9c11-9517ee0409c2.png)

### Block Diagram of the implementation of Linear Regression Model
![image](https://user-images.githubusercontent.com/50255936/110656495-f65c8e00-81fa-11eb-910d-33442eb8a81d.png)

### Classification Accuracy
![image](https://user-images.githubusercontent.com/50255936/110656583-0b392180-81fb-11eb-9202-865ad80c0993.png)

### Confusion Matrix
![image](https://user-images.githubusercontent.com/50255936/110656702-260b9600-81fb-11eb-8d0d-39f16b97ff4d.png)


