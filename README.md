OBJECTIVE:
The objective of this assignment is to implement a two-layer perceptron using the backpropagation algorithm to solve the parity problem. The network will consist of four binary input elements, four hidden units, and one output unit. The desired output is 1 if the input pattern contains an odd number of 1’s, and 0 otherwise. The implementation will use a logistic sigmoid activation function and random initialization of weights and biases. The training will be evaluated based on different learning rates (η), varied from 0.05 to 0.5, with and without a momentum term (α = 0.9), to analyze their effects on the speed and efficiency of convergence. The stopping criterion is defined as achieving an absolute error of 0.05 or less for every input pattern. The outcome will include the number of epochs required for convergence at each learning rate, as well as the effect of momentum on the training speed.

IMPLEMENTATION:
![image](https://github.com/user-attachments/assets/b61592b2-07b2-4a7f-8e36-2d36d5a7410a)

W1: Represents the weights matrix for the connections between the input layer and the hidden layer. Since the input layer has 4 neu- rons and the hidden layer has 4 neurons, the dimensions of W 1 are 4 × 4.
B1: Represents the bias vector for the 4 hid- den neurons. The dimension of B1 is 4 × 1, where each element corresponds to the bias applied to one hidden neuron.
W2: Represents the weights matrix for the connections between the hidden layer and the output layer. The dimensions of W 2 are 4×1.
B2: Represents the bias for the output layer. The dimension of B2 is 1 × 1.

RESULTS:
![image](https://github.com/user-attachments/assets/ea7599be-3bff-47ca-9175-3b60c073e26e)

![image](https://github.com/user-attachments/assets/51819acd-7330-46d7-b393-cff73b4151d6)

![image](https://github.com/user-attachments/assets/80125fdb-b168-4ef9-b25e-68c528bd4e54)

1. Momentum = 0.9 consistently improves convergence, requiring fewer epochs and significantly reducing training time com- pared to Momentum = 0, especially at lower learning rates (0.05 to 0.2).
2. Momentum = 0 experiences instability at low learning rates, with both epochs and training time spiking dramatically, particu- larly at a learning rate of 0.1, in contrast to the smoother performance of Momentum = 0.9.
3. At higher learning rates (0.3 and above), the difference in performance between Mo- mentum = 0 and Momentum = 0.9 be- comes smaller, though Momentum = 0.9 still demonstrates a slight advantage in both epochs and training time.



