### Architecture
INPUT -> [CONV -> RELU -> POOL] * 3 -> [FC -> RELU] -> DROPOUT -> [FC -> RELU] -> OUTPUT


### Hyper-parameters
- Epochs: 100
- Batch size: 256
- Keep probability: 0.5
- Stddev for truncated_normal function: 0.05
- 3 Conv-Pool layers:
    - filters: 32 -> 64 -> 128
    - conv_ksize: (3, 3)
    - conv_strides: (1, 1)
    - pool_ksize: (2,2)
    - pool_strides=(2, 2)
- 2 Fully-Connected layers:
    - nodes in layer 1: 1024
    - nodes in layer 2: 128

### References
* [CS231n note: Convolutional Neural Networks (CNNs / ConvNets)](http://cs231n.github.io/convolutional-networks/)
* [TensorFlow-Examples: CNN](https://github.com/aymericdamien/TensorFlow-Examples/blob/master/examples/3_NeuralNetworks/convolutional_network.py)
* [Image Classification Project Speficiation](https://review.udacity.com/#!/rubrics/723/view)
* [ConvNetJS CIFAR-10 demo](https://cs.stanford.edu/people/karpathy/convnetjs/demo/cifar10.html): architecture and hyper-parameters

### Results
- Training Accuracy= 0.77300
- Testing Accuracy: 0.7626953125
