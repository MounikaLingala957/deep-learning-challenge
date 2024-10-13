{
  "nbformat": 4,
  "nbformat_minor": 0,
  "metadata": {
    "colab": {
      "provenance": [],
      "authorship_tag": "ABX9TyOH1UkPAz0lt5VHnOMc+xXr",
      "include_colab_link": true
    },
    "kernelspec": {
      "name": "python3",
      "display_name": "Python 3"
    },
    "language_info": {
      "name": "python"
    }
  },
  "cells": [
    {
      "cell_type": "markdown",
      "metadata": {
        "id": "view-in-github",
        "colab_type": "text"
      },
      "source": [
        "<a href=\"https://colab.research.google.com/github/MounikaLingala957/deep-learning-challenge/blob/main/README.md\" target=\"_parent\"><img src=\"https://colab.research.google.com/assets/colab-badge.svg\" alt=\"Open In Colab\"/></a>"
      ]
    },
    {
      "cell_type": "code",
      "execution_count": null,
      "metadata": {
        "id": "8DFql_EUFJe_"
      },
      "outputs": [],
      "source": []
    },
    {
      "cell_type": "markdown",
      "source": [
        "# Deep Learning Challenge\n",
        "\n",
        "This repository contains a deep learning project for the nonprofit foundation **Alphabet Soup**, aimed at predicting the success of funding applicants.\n",
        "\n",
        "## Data Preprocessing\n",
        "\n",
        "### Target Variable:\n",
        "- **IS_SUCCESSFUL**: A binary variable indicating whether a charity project was successful (`1`) or not (`0`).\n",
        "\n",
        "### Feature Variables:\n",
        "- All other columns, except **EIN**, **NAME**, and **IS_SUCCESSFUL**, serve as features for the model. These include various characteristics of the charity projects and the organizations behind them.\n",
        "\n",
        "### Variables Removed:\n",
        "- **EIN** and **NAME** were removed from the dataset because they are identifiers that do not contribute to predicting the success of a project. They do not contain any relevant information that would help the model make better predictions.\n",
        "\n",
        "## Compiling, Training, and Evaluating the Model\n",
        "\n",
        "### Neurons, Layers, and Activation Functions:\n",
        "\n",
        "#### Neurons and Layers:\n",
        "- The final neural network model consists of 3 hidden layers with **128**, **64**, and **32** neurons, respectively.\n",
        "- The initial model started with fewer neurons and layers, but complexity was increased to capture more patterns in the data, which improved performance.\n",
        "\n",
        "#### Activation Functions:\n",
        "- **ReLU (Rectified Linear Unit)** was used for the hidden layers to introduce non-linearity and handle complex patterns in the data.\n",
        "- **Sigmoid** activation function was used for the output layer because the task is a binary classification problem.\n",
        "\n",
        "### Model Performance:\n",
        "\n",
        "#### Target Performance:\n",
        "- The target was to achieve an accuracy of at least **75%**.\n",
        "- After multiple optimization attempts, the final model achieved an accuracy of **72%** on the test dataset.\n",
        "\n",
        "#### Steps to Increase Performance:\n",
        "1. **Increased Neurons and Layers**: The model started simple but was made more complex by adding more neurons and layers. This helped capture more detailed patterns from the data.\n",
        "2. **Adjusted Activation Functions**: ReLU was chosen for hidden layers due to its efficiency in deep learning models. The **tanh** function was also tested to handle specific data patterns better.\n",
        "3. **Increased Epochs**: The number of epochs was increased to **150**, allowing the model more time to learn from the data, which contributed to the improved accuracy.\n",
        "\n",
        "## Summary\n",
        "\n",
        "### Overall Results:\n",
        "- The final deep learning model achieved an accuracy of **72%**, which falls short of the target performance of 75%.\n",
        "- While the model shows some capability in predicting the success of charity projects funded by Alphabet Soup, its accuracy is not high enough to be fully reliable for guiding funding decisions.\n",
        "- As it stands, the model may not be the most effective tool for making informed funding choices.\n",
        "\n"
      ],
      "metadata": {
        "id": "649oo1QjFRKE"
      }
    }
  ]
}