# Neural-Network
MNIST digit classification with a Neural Network.

#### [Neural Network](https://github.com/rishab-pdx/Neural-Network/blob/master/digitClassifier.py)
Supervised learning using a Neural Network to predict a function that classisfies MNIST digits.

Neural network structure: The neural network takes in (28x28) 784 inputs, one hidden layer with `n` hidden units (where n is a parameter that can be changed), and 10 output units`(0-9)`. The hidden and output units uses [sigmoid activation function](https://en.wikipedia.org/wiki/Sigmoid_function). The network is fully connected —that is, every input unit connects to every hidden unit, and every hidden unit connects to every output unit. Every hidden and output unit also has a weighted connection from a bias unit, whose value is set to 1.

##### Parameters of the network:
  Input - [28x28 normalized pixels of MNIST digits](https://www.tensorflow.org/versions/r1.0/images/MNIST-Matrix.png)
  
  Number of neurons in the hidden layer - [n](https://github.com/rishab-pdx/Neural-Network/blob/73fa15180185ecadc532e273d36e9a839e4829d3/digitClassifier.py#L32) = 100
  
  Number of epochs - [epochs](https://github.com/rishab-pdx/Neural-Network/blob/73fa15180185ecadc532e273d36e9a839e4829d3/digitClassifier.py#L8) = 50
  
  Learining rate - [eta](https://github.com/rishab-pdx/Neural-Network/blob/73fa15180185ecadc532e273d36e9a839e4829d3/digitClassifier.py#L11) = 0.1
  
  Momentum - [alpha](https://github.com/rishab-pdx/Neural-Network/blob/73fa15180185ecadc532e273d36e9a839e4829d3/digitClassifier.py#L14) = 0.9
  
##### Accuracy vs Parameters

η | α | n | Training Accuracy| Test Accuracy |
--|---|---|------------------|---------------|
0.1|0.9|20|[96%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-1-n-20.png)|[93%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-1-n-20.png)|
0.1|0.9|50|[98%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-1-n-50.png)|[96.8%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-1-n-50.png)|
0.1|0.9|100|[99.6%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-1-n-100.png)|[96.85%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-1-n-100.png)|
0.1|0|100|[99.6%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-2-alpha-0.png)|[97.7%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-2-alpha-0.png)|
0.1|0.25|100|[99.6%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-2-alpha-0.25.png)|[97.7%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-2-alpha-0.25.png)|
0.1|0.5|100|[99.6%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-2-alpha-0.5.png)|[97.6%](https://github.com/rishab-pdx/Neural-Network/blob/master/plots/exp-2-alpha-0.5.png)|

### Dependencies
1. Python
2. Matplotlib
