# -- Multivariate Anomaly Detection for Time Series Data with GANs -- #

# MAD-GAN

This repository contains code for the paper, _[Anomaly Detection with Generative Adversarial Networks for Multivariate Time Series](https://arxiv.org/pdf/1809.04758.pdf)_, by Dan Li, Dacheng Chen, Jonathan Goh, and See-Kiong Ng.

## Overview

We used generative adversarial networks (GANs) to do anomaly detection for time series data.
The GAN framework was **R**GAN that taken from the paper, _[Real-valued (Medical) Time Series Generation with Recurrent Conditional GANs](https://arxiv.org/abs/1706.02633).
Please refer to https://github.com/ratschlab/RGAN for the original code.

## Quickstart

- Python3

- To train the model:
  $ cd MAD-GAN-master
  $ python RGAN.py --settings_file kdd99

- To do anomaly detection:
  $ cd MAD-GAN-master
  $ python AD.py --settings_file kdd99_test
  $ python AD_Invert.py --settings_file kdd99_test

## Data

We apply our method on the SWaT and WADI datasets in the paper, however, we didn't upload the data in this repository. Please refer to https://itrust.sutd.edu.sg/ and send request to iTrust is you want to try the data.

In this repository we used kdd cup 1999 dataset as an example. You can also down load the original data at http://kdd.ics.uci.edu/databases/kddcup99/kddcup99.html
