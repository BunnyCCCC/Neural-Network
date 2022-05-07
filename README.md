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
This project focused on experimenting five different CNN models and trying to get a higher classification accuracy for CIFAR-10.
- The first model has two convolutional layers followed by a max pooling layer.
- The second model reduce the max pooling size to half and add the dropout rate after the max pooling layers. Also, the fully-connected layer has an increased neuron size of 128.
- The third model add two more convolutional layers and group them as 2 convolutional layers + 1 max pooling layer. The dropout rate has been adjusted to prevent overfitting.
- The fourth model reduces the max pooling stride and increases the fully-connected layer size to capture more information during training.
- The fifth model increases the convolutional layers to a total of 6 layers(3 sets, each set has 2 convolutional layers + 1 batch normalization + 1 max pooling layer). The fully connected layer size has been reduced back to 128 and the stride of max pooling layer has been increased to 4 to reduce the training time.
<a/>
  
The final accuracy has been improved from 68.87% to 82.2%.  
The visualization of filters in convolutional layers and visualization of top 9 feature maps were created to help adjusting the parameters and finding the balance among overfitting, underfitting, training accuracy, and GPU time.

