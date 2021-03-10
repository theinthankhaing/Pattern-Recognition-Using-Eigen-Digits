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

Eigen - Digits Images
![image](https://user-images.githubusercontent.com/50255936/110647209-982bad00-81f2-11eb-8c20-c33cea625af0.png)
___________________________________________________________________________
## Image Reconstruction
Original Test Images are projected into the subspace spanned by the top 30 eigenvectors by usign the following equation
![image](https://user-images.githubusercontent.com/50255936/110647720-0a9c8d00-81f3-11eb-802e-e4c63ea7baaf.png)
