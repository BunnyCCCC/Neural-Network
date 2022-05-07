# Neural-Network
Mini projects about application of neural networks
------------------------------------------------------------------------------------------------------------




**Function Approximation**\
This project focused on experimenting function approximation using neural network regression models.
All of the different models used non-linear tanh activation function with different neuron sizes(2 to 50),
and different optimizers.
Compared Mean Squared Errors for three optimization methods, and CPU time with early stoppings
Finally concluded that 8 neurons in the hidden layer is the optimum size for this function approximation.
The optimizer of RMSprop with early stopping, batch size of 10 and trained for 1000 epoches achieved optimum 
result for this function approximation experiment.

**Multilayer Feedforward Network for Pattern Recognition**\
This project focused on experimenting pattern recognition with multilayer feedforward network.
Each target letter was created using pixels represented by 0s and 1s in a 7 by 5 matrix, each distorted letter 
was created with 1 to 3 pixels flipped.
First the model was trained with target letters for hidden layer sizes ranging from 5 to 25. The training is 
for 5000 epoches and batch size of 10 for each hidden layer size.
Then I compared with 2 different training methods and plot the training errors against number of epoches:
- regular training method with target letters.
- 3-steps training method: first with target letters, then with distorted letters, and finally with target 
letters again.  
<a/>
  
Lastly, I tested 2 training methods on random generated test data which is randomly flipped 0 to 3 pixels for
each input. The model was trained 5000 epoches for both methods and plot the recognition error percentage against noise levels with these two different methods.

**Convolutional Neural Neywork for CIFAR-10**\
to do...
