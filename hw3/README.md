# CSC585 Homework3
This folder contains the code of CSC585 homework 3. There are two Differentiable Neural Computer (DNC) implementations and an LSTM implementation. If you have any problems running the code, please contact me freely.

## DNC Implementation on bAbI
The code is in folder "DNC_bAbI_docker". The code is copied from [DNC Mostafa](https://github.com/Mostafa-Samir/DNC-tensorflow), where the author implemented a DNC introduced in [this paper](https://www.nature.com/articles/nature20101.epdf?author_access_token=ImTXBI8aWbYxYQ51Plys8NRgN0jAjWel9jnR3ZoTv0MggmpDmwljGswxVdeocYSurJ3hxupzWuRNeGvvXnoO8o4jTJcnAyhGuZzXJ1GEaD-Z7E6X_a9R-xqJ9TfJWBqz) and test it on [bAbI tasks](https://research.fb.com/downloads/babi/). This is implemented in tensorflow. 

User can either run this by docker or by setting up his own environment.

### Set up Environment Manually
The following libraries are needed:
``python 2.7``
``numpy==1.12.0``
``tensorflow==0.12.0``. 
After correctly installing the libraries, one needs to run:
`python test.py`
The DNC will load a trained model of 30,000 iterations. Note that loading model only supports CPU. If you have a GPU-version tensorflow, you need to train the model again. To retrain the model, one just needs to run ``python train.py --iterations=XXXX``.
### Run the Script with Docker
Just run the script by typing the command in ``run_docker.sh``.

## DNC Implementation on MNIST
The code is in folder "DNC_MNIST_docker". The code trains a DNC to reproduce MNIST hand-written digit. The experiment is described in detail in the appendix of the report. Original code is from [here](https://github.com/llSourcell/differentiable_neural_computer_LIVE).

Although I tried to wrap the code in docker, it hangs when I try to run it through docker (but with no error). If you want to run the script you will need to set up the environment yourself. The libraries are ``python 3.6``, ``numpy==1.12.0``, ``tensorflow==1.10.0``. The just type ``python DNC_MNIST.py``.

## LSTM Implementation on MNIST
The code is stored in "DNC_MNIST_docker" folder (but docker is not supported for this implementation), and the script name is "3_Normal_LSTM_MNIST.py". This implementation trains an LSTM to reproduce MNIST hand-written digit. The details of the experiment are provided in the appendix in the report. To run the script, just type ``python 3_Normal_LSTM_MNIST.py``.



