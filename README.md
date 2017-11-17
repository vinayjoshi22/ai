This repository contains code for different neural networks for example, mlp, gan, etc. This work is in progress and I'll keep adding new code as when I build one successfully. Any comments/suggestions/bugs-reports are most welcome.

- [MLP](https://github.com/vinayjoshi22/ai/tree/master/ann/mlp) : Code contains python class for mlp. Network.ipynb is an example file demonstrating use of class network.py that implements mlp. Simple use for [MNIST dataset](https://pjreddie.com/projects/mnist-in-csv/) network is as follows,

Import network into the python code
`import network as Network`

Build the network with architecture desired
```
mnist = Network.Network(layer_units,
                        learning_rate,
                          epochs,
                          x_train,
                          y_train,
                          x_test,
                          y_test,
                          x_val,
                          y_val,
                          learning_rate_set=None)
```
Train network - returns training progress of the network

`mnist.train()`

Test network - returns performance of the network on test set
`mnist.test()`

To access the parameters of the network
```
mnist.weights
mnist.bias
```
To reevaluate networks
`mnist.accuracy(x_train,y_train) // returns train accuracy`

Note: To run sample for MNIST you should download [MNIST dataset](https://pjreddie.com/projects/mnist-in-csv/) and put it in the same folder as [Network.ipynb](https://github.com/vinayjoshi22/ai/blob/master/ann/mlp/python/Network.ipynb). You can use iPython to run this interactively or directly in in command prompt.
