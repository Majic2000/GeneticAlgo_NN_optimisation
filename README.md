# GeneticAlgo_NN_optimisation

Title: Training Feed-Forward Multi-Layer Perceptron Networks using Evolutionary Algorithms for Function Approximation

Abstract:
This work aims to train feed-forward multi-layer perceptron networks with two hidden layers to approximate a specific function using evolutionary algorithms. The function to be approximated is y = sin(3.5x1 + 1.0)cos(5.5x2), where x1 and x2 are in the range [-1, 1]. The implementation is performed in Python, including NumPy, PyTorch, and DEAP.

Firstly, the function is visualized with a 3D surface plot. Then, 1100 samples of x1 and x2 are randomly generated within the range, and the corresponding y values are calculated. The dataset is divided into a training set (1000 samples) and a test set (100 samples), both of which are visualized separately in 3D graphics.

A fully connected neural network with six hidden neurons in each hidden layer is implemented. Sigmoid activation function is used for hidden neurons, while the output neuron utilizes a linear activation function. The code for creating the network is provided.

Two functions, weightsOutofNetwork and weightsIntoNetwork, are implemented to extract and insert weights of the network. A test is conducted to verify the correct retrieval and insertion of weights, highlighting any changes made.

A binary coded genetic algorithm with Gray coding is employed to optimize the network's weights by minimizing the mean squared error on the training dataset. Hyperparameters are experimented with to achieve good results, and a plot of the training and test errors across generations is presented.

Additionally, a 3D surface plot is generated to visualize the function implemented by the neural network. A function is implemented to convert weights into a chromosome using Gray coding, ensuring weights are within the range [-20, 20]. A test is conducted to validate the conversion process.

The Rprop learning algorithm is embedded in the genetic algorithm as a local search method, utilizing the Lamarckian learning approach. The code is extended to implement 30 iterations of local search in each generation. The training and test errors across generations, along with a 3D surface plot of the function implemented by the neural network, are presented.

Furthermore, the Baldwinian learning approach replaces the Lamarckian approach, and the results are compared and discussed. The training and test errors across generations, along with the 3D surface plot, are shown and analyzed for differences and potential reasons.

Overall, this reserach project provided me with hands-on experience in using evolutionary algorithms and neural networks for function approximation, showcasing the implementation, optimization, and analysis of the network's performance using different learning approaches.





