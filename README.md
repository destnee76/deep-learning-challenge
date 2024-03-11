# deep-learning-challenge
## Report on the Neural Network Model Performance

- [Link to Colab Notebook](https://colab.research.google.com/drive/1nfnbZBiQHha0qtqWaPtwAPVLZIuzOKPJ?usp=drive_link)
- [Link to Optimization Notebook](https://colab.research.google.com/drive/1TKV1IteNaA5aT0YM_2MX_gYY4aXctER7?usp=drive_link)

## Overview of the Analysis:
The purpose of this analysis is to develop a deep learning model using a neural network to predict the success of charitable organizations based on various features such as application type, affiliation, classification, etc. The model is trained on a dataset provided by Alphabet Soup.

## Results:

### Data Preprocessing:

#### Target(s) and Features:
- **Target(s):**
  - `IS_SUCCESSFUL`: Indicates whether the charity donation was used effectively (1) or not (0).

- **Features:**
  - All columns except `IS_SUCCESSFUL` are considered features.

#### Removed Variables:
- `EIN` and `NAME` columns were removed as they are not beneficial for predictive modeling.

### Compiling, Training, and Evaluating the Model:

#### Model Architecture:
- **Neurons and Layers:**
  - Initial model: 50 neurons in the first hidden layer and 30 neurons in the second hidden layer.
  - Modified model 1: 64 neurons in the first hidden layer, 32 neurons in the second hidden layer.
  - Modified model 2: 20 neurons in each of the two hidden layers.
  - Modified model 3: 50 neurons in the first hidden layer, 30 neurons in the second hidden layer, and 10 neurons in the third hidden layer.

- **Activation Functions:**
  - Initial model and Modified model 1: `relu` activation function in hidden layers and `sigmoid` activation function in the output layer.
  - Modified model 2: `tanh` activation function in the first two hidden layers, and `sigmoid` activation function in the output layer
  - Modified model 3: `sigmoid` activation function in the first two hidden layers, `tanh` activation function in the third hidden layer, and `sigmoid` activation function in the output layer.

#### Model Performance:
- **Initial Model:**
  - Accuracy: 72.50%
  - Loss: 0.5551

- **Modified Model 1:**
  - Accuracy: 72.67%
  - Loss: 0.5517

- **Modified Model 2:**
  - Accuracy: 72.30%
  - Loss: 0.5515

- **Modified Model 3:**
  - Accuracy: 72.66%
  - Loss: 0.5515

### Summary:
The deep learning models achieved an accuracy ranging from approximately 72.50% to 72.67%. Although the modifications made to the architecture did not lead to a significant improvement in model performance, they demonstrate the flexibility of neural networks in accommodating various configurations. 

To further enhance model performance, more advanced techniques could be explored such as adjusting learning rates, experimenting with different optimizers, or implementing more complex architectures like convolutional neural networks (CNNs) or recurrent neural networks (RNNs) if the nature of the data warrants it. Additionally, ensemble methods such as bagging or boosting could be employed to combine the strengths of multiple models for better predictive accuracy. Regularization techniques like dropout or L2 regularization can also be utilized to prevent overfitting. Further exploration and experimentation are recommended to refine the model and potentially improve its predictive power.
