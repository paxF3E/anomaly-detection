<p align="center">
    <a href="https://github.com/paxF3E/anomaly-detection">
        <img src="https://github.com/paxF3E/anomaly-detection/blob/main/logo.jpg" alt="[Project Logo]" width="30%"> 
    </a>
</p> 

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


## DIVERSION 2k23
### This project is part of Diversion 2k23

<p align="center">
    <a href="https://diversion.tech/">
        <img src="https://github.com/acm-iem/Readme-template/blob/main/Logos/Diversion%20Full%20Logo%20White.png" width="30%">
    </a>
</p>

<h1 align="center"> DIVERSION 2k23 🎉</h1>

<div align="center">
   
   [![GitHub issues](https://img.shields.io/github/issues/chaitak-gorai/Project-Template-Hacktoberfest22?color=pink&logo=github)](https://github.com/paxF3E/anomaly-detection/issues)        [![GitHub PRs](https://img.shields.io/github/issues-pr/chaitak-gorai/Project-Template-Hacktoberfest22?style=social&logo=github)](https://github.com/paxF3E/anomaly-detection/pulls)                    [![GitHub forks](https://img.shields.io/github/forks/chaitak-gorai/Project-Template-Hacktoberfest22?logo=git)](https://github.com/paxF3E/anomaly-detection/network)
   
   <a href="https://github.com/paxF3E/anomaly-detection/contributors"><img alt="GitHub contributors" src="https://img.shields.io/github/contributors/chaitak-gorai/Project-Template-Hacktoberfest22?color=2b9348"></a>
<a href="https://github.com/paxF3E/anomaly-detection/blob/master/LICENSE"><img src="https://img.shields.io/github/license/chaitak-gorai/Project-Template-Hacktoberfest22?color=2b9348" alt="License Badge"/></a>
</div>

## 🗣 DIVERSION 2k23 encourages participation in the open source community, which grows bigger every year. Complete the challenge and win amazing rewards.

📢 **Register [here](https://diversion.tech/) for DIVERSION 2k23 and start contributing to the projects.**

## Features to be developed during the event.
   [Add Feature list]
   
## DIVERSION 2k23 Contribution Rules
- Pull requests can be submitted to any opted-in repository on GitHub or GitLab.
- The pull request must contain commits you made yourself.
- If a maintainer reports your pull request as spam, it will not be counted toward your participation in Hacktoberfest.
- If a maintainer reports behavior that’s not in line with the project’s code of conduct, you will be ineligible to participate.
- To get a shirt, you must make four approved pull requests (PRs) on opted-in projects between October 1-31 in any time zone.
- This year, the first 40,000 participants can earn a T-shirt.
---

## Contribute
   ## There are DIVERSION 2k23 contributor guidelines as well as individual project guidelines. 
   ### Do Read - [Code of Conduct](https://github.com/acm-iem/Readme-template/blob/main/CODE_OF_CONDUCT.md)
   ### Jump to - [DIVERSION 2k23 guidelines](https://docs.google.com/document/d/1D7bn0rLv1dP6DAmEnsI8qBLjQrWTdhp0e5ZVy8OFHjc/edit?usp=sharing) (updated)
Why not start your open source journey by merging some codes here. It will be very great if you review the code and  find some bugs and issues.

## Steps for a successful commit :zap:
- Choose any of the **Ways to contribute** for contribution.
- Create a PR and commit by creating a new branch (:warning: Avoid commiting to the main)
- Be patience it might take time for the maintainers to review your PR.
- Congratulations on a successful merge.
- You can add your name to contributors list.


 ### Ways to Contribute 
  * Find a bug by running the project locally
  * Solve the [issues](https://github.com/acm-iem/Readme-template/issues) which are already set up
  * Sugget some change or create your own isssue
  *  Create documentation like site structure, how to write a blog,etc
  *  Indent/Beautify/Modify codes.

### List of Contributors
   After a successful PR merge during the event add the contributor name to this list.
   
Thank You! Keep Contributing :octocat:
