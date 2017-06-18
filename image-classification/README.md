### Architecture
INPUT -> [CONV -> RELU -> POOL] * 3 -> FLAT -> DROPOUT -> [FC -> RELU] * 2 -> DROPOUT -> OUTPUT

### 3 Conv-Pool layers:
- filters: 32 -> 64 -> 128
- conv_ksize: (3, 3)
- conv_strides: (1, 1)
- pool_ksize: (2,2)
- pool_strides=(2, 2)
### 2 Fully-Connected layers:
- number of neurons: 2048

### Other Hyper-parameters
- Epochs: 10
- Batch size: 128
- Keep probability: 0.3
- Stddev for truncated_normal function: 0.05

### References
CS231n note: Convolutional Neural Networks (CNNs / ConvNets)
TensorFlow-Examples: CNN
Image Classification Project Speficiation
ConvNetJS CIFAR-10 demo: architecture and hyper-parameters

### Results
- Training Accuracy: 0.74480
- Testing Accuracy: 0.73170
