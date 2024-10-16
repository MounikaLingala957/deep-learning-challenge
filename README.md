# Deep Learning Challenge

This repository contains a deep learning project for the nonprofit foundation **Alphabet Soup**, aimed at predicting the success of funding applicants.

## Data Preprocessing

### Target Variable:
- **IS_SUCCESSFUL**: A binary variable indicating whether a charity project was successful (`1`) or not (`0`).

### Feature Variables:
- All other columns, except **EIN**, **NAME**, and **IS_SUCCESSFUL**, serve as features for the model. These include various characteristics of the charity projects and the organizations behind them.

### Variables Removed:
- **EIN** and **NAME** were removed from the dataset because they are identifiers that do not contribute to predicting the success of a project. They do not contain any relevant information that would help the model make better predictions.

## Compiling, Training, and Evaluating the Model

### Neurons, Layers, and Activation Functions:

#### Neurons and Layers:
- The final neural network model consists of 3 hidden layers with **128**, **64**, and **32** neurons, respectively.
- The initial model started with fewer neurons and layers, but complexity was increased to capture more patterns in the data, which improved performance.

#### Activation Functions:
- **ReLU (Rectified Linear Unit)** was used for the hidden layers to introduce non-linearity and handle complex patterns in the data.
- **Sigmoid** activation function was used for the output layer because the task is a binary classification problem.

### Model Performance:

#### Target Performance:
- The target was to achieve an accuracy of at least **75%**.
- After multiple optimization attempts, the final model achieved an accuracy of **72%** on the test dataset.

#### Steps to Increase Performance:
1. **Increased Neurons and Layers**: The model started simple but was made more complex by adding more neurons and layers. This helped capture more detailed patterns from the data.
2. **Adjusted Activation Functions**: ReLU was chosen for hidden layers due to its efficiency in deep learning models. The **tanh** function was also tested to handle specific data patterns better.
3. **Increased Epochs**: The number of epochs was increased to **150**, allowing the model more time to learn from the data, which contributed to the improved accuracy.

## Summary

### Overall Results:
- The final deep learning model achieved an accuracy of **72%**, which falls short of the target performance of 75%.
- While the model shows some capability in predicting the success of charity projects funded by Alphabet Soup, its accuracy is not high enough to be fully reliable for guiding funding decisions. 
- As it stands, the model may not be the most effective tool for making informed funding choices.

