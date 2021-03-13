# CS6910

## Assignment 1
Dataset : fashion mnsit  
**Optimizers used for training the model[backpropagation]:**     
    &nbsp;&nbsp;&nbsp;stochastic gradient descent, momemtum based gradient descent,nestrov gradient descent,rmsprop, adam, nadam  
**Activation Functions used in hidden layers:**      
    &nbsp;&nbsp;&nbsp;sigmoid, tanh,relu    
 **Softmax function used at the final output layer**    
 **Layers used in the network**   
    &nbsp;&nbsp;&nbsp;Option 1: [784,128,64,10]  
    &nbsp;&nbsp;&nbsp;Option 2:[784,32,32,32,10]  
 **Error functions used **    
    cross entropy and mse  
      
    
 **function name ----> description**  
      1)sigmoid(x) ------>code for sigmoid function    
      2)sigmoid_dif(x)---------> code for the differentiation of sigmoid function    
      3)tanh(x)---> code for tanh function  
      4)tanh_dif(x)------> code for differentiation of tanh function  
      5)relu(x)----> code for relu function    
      6)relu_dif(x)------> code for differentiation of relu function    
      7)softmax(x)----> code  for softmax function    
      8)initialize_network(layer_size_list,mthd)--------> used to initialize the weights and biases in two ways i.e random and xavier    
      9)forward_propagation(x,weights,bias,mthd)-------> code for forward propagation method    
      10)back_propagation(x,y,weights,bias,mthd)-------> code for backward propagation method    
      11)stochastic_gradient_descent(weights,bias,epochs,layers_size_list,train_images,train_labels,learning_rate,mthd,alpha=0,batch_size=10)-------> code for stochastic    gradient   descent    
      12)momentum_gradient_descent(weights,bias,epochs,layers_size_list,train_images,train_labels,learning_rate,mthd,alpha=0)-------> code for momentum based gradient descent    
      13)nestrov_gradient_descent(weights,bias,epochs,layers_size_list,train_images,train_labels,learning_rate,mthd,alpha=0)-----> code for nestrov gradient descent    
      14)rmsprop(weights,bias,epochs,layers_size_list,train_images,train_labels,learning_rate,mthd,alpha=0) ---------> code for rmsprop    
      15)adam(weights,bias,epochs,layers_size_list,train_images,train_labels,learning_rate,mthd,alpha=0)----> code for adam    
      16)nadam(weights,bias,epochs,layers_size_list,train_images,train_labels,learning_rate,mthd,alpha=0)-------> code for nadam    
      17)mse(pred,label)-----> code for mean squared error loss calculation
      18)cross_entropy(pred,label)----> code for cross entropy loss calculation
      19)test_accuracy(weights,bias,test_images,test_labels,mthd)--------> code to calulate the accuracy obtained from training data set
      20)train()----> code which starts the training of the model. Using train() method all the above functions will be called recursively as and when needed according to the 
                      configuration selected by sweep
             
 

   

