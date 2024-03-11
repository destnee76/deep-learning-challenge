# deep-learning-challenge
# Report on the Neural Network Model Performance
## Overview of the Analysis:
The analysis aimed to build a deep learning model using a neural network to predict the success of charitable organizations based on various features provided by Alphabet Soup. Three attempts were made, progressively adjusting the model's architecture to improve performance.

## Results:
### Building and Testing the Model:

### Original Attempt:
[Link to Colab Notebook](https://colab.research.google.com/drive/1nfnbZBiQHha0qtqWaPtwAPVLZIuzOKPJ?usp=drive_link)
- **Architecture:**
  - Two hidden layers with 50 and 30 neurons respectively.
  - Activation function: `relu` for the first and second hidden layers, and `sigmoid` for the output layer.

- **Performance:**
  - Accuracy: 72.50%
  - Loss: 0.5575

### Additional Attempts:
[Link to Optimization Notebook](https://colab.research.google.com/drive/1TKV1IteNaA5aT0YM_2MX_gYY4aXctER7?usp=drive_link)
### Attempt 1:
- **Architecture:**
  - Two hidden layers with 64 and 32 neurons respectively.
  - Activation function: `relu` for hidden layers and `sigmoid` for the output layer.

- **Performance:**
  - Accuracy: 72.59%
  - Loss: 0.5551

### Attempt 2:
- **Architecture:**
  - Two hidden layers with 20 neurons each.
  - Activation function: `tanh` for hidden layers and `sigmoid` for the output layer.

- **Performance:**
  - Accuracy: 72.62%
  - Loss: 0.5517

### Attempt 3:
- **Architecture:**
  - Three hidden layers with 50, 30, and 10 neurons respectively.
  - Activation function: `sigmoid` for the first two hidden layers, `tanh` for the third hidden layer, and `sigmoid` for the output layer.

- **Performance:**
  - Accuracy: 72.76%
  - Loss: 0.5515

## Summary:
The initial attempt achieved an accuracy of 72.50%, which was slightly improved upon in the subsequent attempts. While the adjustments in the architecture did not result in significant performance gains, they highlight the iterative nature of model development. Further experimentation with hyperparameters, activation functions, and additional layers could potentially enhance the model's predictive power. Additionally, exploring ensemble methods and regularization techniques may contribute to improving model performance.
