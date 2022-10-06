## Anomaly Detection System
- anomaly detection system to detect outliers in server nodes using Gaussian model
- implemented on two sets of data
  1. dataset with two features: Latency and Throughput
  2. higher dimensional dataset with a set of 11 features
  
### Dependencies
- jupyter with python 3.10.6 64-bit kernel
- python libraries: pandas, matplotlib, numpy, pylab

### Dataset
1. 2-dimensional dataset
  - `data_train.csv`: training set for the 2-D data
  - `data_val.csv`: validation set including `X_val` and `y_val`; separated after loading dataset
2. 11-dimensional dataset
  - `data2_X.csv`: training set with 11 features
  - `data2_Xval.csv`: validation set with 11 features
  - `data2_yval.csv`: validation labels to assess the model trained on the higher dimensional dataset

### Performance Measures
- performance of this unsupervised Gaussian model is determined using the F1-score for every iteration till it saturates to its optimum
- the model is trained over the training set to learn the parameters `mu` and `sigmasq` denoting the dataset's mean and variance
- validation set is fed to the model using the learnt `mu` and `sigmasq` to learn the new parameter `epsilon` by maximizing the F1 score
- using the learnt parameter `epsilon` outliers are detected in the dataset
  
### Performance Goals
1. 2-dimensional dataset
  - optimum epsilon expected: `8.99e-05`
  - best F1 score: `0.875000`
2. 11-dimensional dataset
  - optimum epsilon expected: `1.38e-18`
  - best F1 score: `0.615385`
