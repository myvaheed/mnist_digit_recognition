# mnist_digit_recognition 
## Digit recognition from MNIST Dataset via convolutional neural network based on PyTorch library 
- Average validation accuracy : 0.99 
- Result is got via CNN based on PyTorch. 
- Data split: 0.8 
- Num epochs: 20 

## Sequential Architecture:

**Convolutional Block** 
- Conv2d(32) 
- ReLU 
- Conv2d(64) 
- ReLU 
- MaxPool2d(2) 
- Dropout(0.25)

**Linear Block** 
- Dense(128) 
- BatchNorm1d 
- ReLU 
- Dropout(0.5) 
- Dense(64) 
- BatchNorm1d 
- ReLU 
- Dropout(0.5) 
- Dense(10) 

## Training params:
- Optimizer: Adadelta
>- coefficient used for computing a running average of squared gradients (rho) 0.95
>- learning rate = 1.0
>- eps = 1e-6 
- Loss function: Cross Entropy 

![](https://www.googleapis.com/download/storage/v1/b/kaggle-user-content/o/inbox%2F3989029%2F2df77def51d11d8421578e03a8c122a5%2Fmnist_result.png?generation=1573479974868019&alt=media)
