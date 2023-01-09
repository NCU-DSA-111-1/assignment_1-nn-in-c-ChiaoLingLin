# Simple network that can learn XOR 
##### Data Structure Assignment 1
##### 通訊二110503504林巧翎

This is assignment 1

## Compile 
```
$ make

gcc -Wall -g -pedantic -std=c99   -c -o ann.o ann.c
gcc -Wall -g -pedantic -std=c99   -c -o layer.o layer.c
gcc   train.o ann.o layer.o  -lm -o train


```
## Run
```
./train

```

## Release

```
Big data machine learning.

--------------------------
PART I - Creating a layer.

Trying to layer_create.
Running layer_init.
Here are some of the properties:
  num_outputs: 2
   num_inputs: 0
   outputs[0]: 0.000000
   outputs[1]: 0.000000

Creating second layer.
Running layer_init on second layer.
Here are some of the properties:
  num_outputs: 1
   num_inputs: 2
   weights[0]: -0.466530
   weights[1]: -0.170036
    biases[0]: 0.000000
   outputs[0]: 0.000000

Computing second layer outputs:
Here is the new output:
   outputs[0]: 0.500000

Freeing both layers.

--------------------------
PART II - Creating a neural network.
2 inputs, 2 hidden neurons and 1 output.

 * - * \ 
         * - 
 * - * / 

Initialising network with random weights...
The current state of the hidden layer:
  weights[0][0]: 0.190636
  weights[0][1]: -0.077513
  weights[1][0]: -0.293735
  weights[1][1]: -0.249872
  biases[0]: 0.000000
  biases[1]: 0.000000
  outputs[0]: 0.000000
  outputs[1]: 0.000000
Current random outputs of the network:
  [0, 0] -> 0.562199
  [0, 1] -> 0.554171
  [1, 0] -> 0.562062
  [1, 1] -> 0.554057

Training the network...
The current state of the hidden layer:
  weights[0][0]: -12.419653
  weights[0][1]: -23.432250
  weights[1][0]: -12.561441
  weights[1][1]: -23.574103
  biases[0]: 3.415144
  biases[1]: 14.394006
  outputs[0]: 0.000000
  outputs[1]: 0.000000

After training magic happened the outputs are:
  [0, 0] -> 0.000145
  [0, 1] -> 0.604772
  [1, 0] -> 0.604736
  [1, 1] -> 0.605006
```

