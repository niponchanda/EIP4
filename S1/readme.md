Score: [0.038388804367152946, 0.9917]

Definitions

Convolution:
            Convolution is a operation on two matrix that produces a third matrix.
            Convolution and correlation are same 99 % of times.
            
Kernels/Filters:
            A kernel is a matrix which convolve with input matrix and extract features.
            Mostly 3x3 kernel is used, because of its advantages.
            
Epochs:
       Epoch is the number of time it is going to dataset.
       
Feature maps:
       A collection of similar information, when we convolve input matrix with kernel, 
       we get feature maps.
       
Activation function: 
      Relu is the default activation function. It is used to enhance the network.
      
Receptive field:
      Receptive field is the convolution of input matrix and kernel. There are local
      receptive field and global receptive field. The receptive field of the last 
      layer should be atleast the size of the object.
      
3x3 convolution:
      Advantages of 3x3 convolution:
      --> It can use 2x2 as well as 3x3.
      --> Odd size kernel.
      --> Only 18 parameters.
  
1x1 convolution:
          1x1 convolution combines those features which are contextually linked with 
          each other. It is like DJ, it combines.
