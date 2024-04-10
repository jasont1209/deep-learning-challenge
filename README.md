# deep-learning-challenge

## NEURAL NETWORK MODEL REPORT:
 
## Overview of the analysis:
The purpose of this analysis is to create a tool that can help Alphabet Soup to select applicants for funding with the best chance of success in their ventures. Features in the provided dataset by Alphabet Soup will be used to create a binary classifier to predict if applicants will be successful if funded by Alphabet Soup.

## Results:

## Data Preprocessing

### What variable(s) are the target(s) for your model?
The target is "y", which is the "IS_SUCCESSFUL" Column.

### What variable(s) are the features for your model?
"X" is the Features for the model, which is everything except "IS_SUCCESSFUL" column. 

### What variable(s) should be removed from the input data because they are neither targets nor features?
"EIN" and "NAME" were removed from input data because they are neither targets nor features.

## Compiling, Training, and Evaluating the Model

### How many neurons, layers, and activation functions did you select for your neural network model, and why?
For the first model: 
    - 2 Hidden layers and an outer layer;
        - layer 1 with 80 neuron and tanh activation
        - layer 2 with 30 neuron and sigmoid activation
        - output layer with sigmoid activation
        - adam optimizer
    - Model training with 25 epochs
    - Achieved accuracy: 0.7283

for Optimization attempt #1:
    - 2 Hidden layers and an outer layer;
        - layer 1 with 100 neuron and tanh activation
        - layer 2 with 50 neuron and sigmoid activation
        - layer 3 with 50 neuron and relu activation
        - output layer with sigmoid activation
        - adam optimizer
    - Model training with 25 epochs
    - Achieved accuracy: 0.7283

for Optimization attempt #2:
    - 2 Hidden layers and an outer layer;
        - layer 1 with 150 neuron and relu activation
        - layer 2 with 100 neuron and relu activation
        - layer 3 with 50 neuron and relu activation
        - output layer with sigmoid activation
        - adam optimizer
    - Model training with 50 epochs
    - Achieved accuracy: 0.7296

- for Optimization attempt #3:
    - 2 Hidden layers and an outer layer;
      - layer 1 with 200 neuron and relu activation
        - layer 2 with 100 neuron and relu activation
        - layer 3 with 50 neuron and relu activation
        - output layer with sigmoid activation
        - adam optimizer
    - Model training with 50 epochs
    - Achieved accuracy: 0.7291 


### Were you able to achieve the target model performance?
I was not able to achieve target model performance, the highest is 72.96%
### What steps did you take in your attempts to increase model performance?
I tried to use different number of layers, different types of activations and different number of epochs.
### Summary: 
The difference in accuracy between the optimization attempts were minimal. More attempts at different modifications would be needed for a proper recommendation
