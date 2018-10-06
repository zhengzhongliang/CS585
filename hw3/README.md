# CSC585 Homework3
This folder contains the code of CSC585 homework 3. There are two Differentiable Neural Computer (DNC) implementations and an LSTM implementation. 

## DNC Implementation on bAbI
The code is in folder "DNC_bAbI_docker". The code is copied from [DNC Mostafa](https://github.com/Mostafa-Samir/DNC-tensorflow), where the author implemented a DNC introduced in [this paper](https://www.nature.com/articles/nature20101.epdf?author_access_token=ImTXBI8aWbYxYQ51Plys8NRgN0jAjWel9jnR3ZoTv0MggmpDmwljGswxVdeocYSurJ3hxupzWuRNeGvvXnoO8o4jTJcnAyhGuZzXJ1GEaD-Z7E6X_a9R-xqJ9TfJWBqz) and test it on [bAbI tasks](https://research.fb.com/downloads/babi/). This is implemented in tensorflow. 

User can either run this by sing docker or by setting up his own environment.

### Set up Environment Manually
The following libraries are needed:
"python 2.7"
"numpy==1.12.0"
"tensorflow==0.12.0"
After correctly install the libraries, one need to run:
"python test.py"
The DNC will load a trained model of 30,000 iterations. Note that loading model only supports CPU. If you have a GPU-version tensorflow, you need to train the model again. The training of model is clarified in [this link](https://github.com/Mostafa-Samir/DNC-tensorflow/tree/master/tasks/babi).

### Run the Script with Docker
Just run the script by typing the command in "run_docker.sh".

