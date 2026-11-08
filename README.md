# ATDL_assignment3_code

This repository contains the code used to extend the experiments in Sakabe et al. (2026) to include MLPs with 2-bit and 4-bit weight precisions. 

## Code files
The experimental files consists of three notebooks as well as three modules implemented by Saintslab in https://github.com/saintslab/QuBD.

### `neural_model.ipynb`

This file contains the code for preprocessing and splitting the MNIST data into training and valdiation sets as described in the assignemnts. Neural network setup and training loops are also contained.

All experimental runs used this file as template. The model specifications were altered as needed for all experimental setups. 

### `shuffled_MNIST.ipynb`

This file contains mostly the same code as neural_model.ipynb, but the MNIST training labels are shuffled. 

### `analysis.ipynb`

This notebook performs all correlation analyses and calculates mean and standard devation of training accuracies. The plots of metrics as a function of epochs is also created in this notebook. The notebook is designed to be placed in the same directory as `neural_model.ipynb` and reads the files output from `neural_model.ipynb`.
