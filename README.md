# Self-Driving-Car

## PROBLEM STATEMENT
Steering wheel angle predictions using dashcam images of the car.


## Research Objectives

To improve efficiency and accuracy of model
To relate to real life problem and solve it

## CNN Model
Data loaded in batches of size 100
Adam optimizer is used for training 
The activation function is used in this model is tanh. 
5 Convolutional Layer with some stride and padding and 3 Fully Connected layer.

Accuracy of CNN Model
Loss is about  4.95%.
The model was able to detect useful road features on its own. As seen in Figure 9 there is a stark difference in the validation Mean Square Error (MSE) loss of the model after 30 epochs.
The model is able to clone the behavior of human driver quite efficiently.





## CNN + Transfer Learning
In transfer learning it  take a model which was trained on a large dataset and transfer its weights and  knowledge to a smaller dataset.
Resnet50 [14] model is used to train the model.
Resnet50 is a 50 layer Residual Network

Accuracy 
Train and Test Loss is about 7%

## Comparison of Models
Prefer simple CNN model over CNN+transfer learning model 

As seen in the figure first loss is decreased and Even after increasing the epochs loss is not decreasing further.
This may happen due to  vanishing gradients.
So dealing with vanishing gradient problem is very important if this model is going to be applied.

## SIMULATION
file:///home/hp/Pictures/Screenshot%20from%202022-07-27%2000-45-28.png![image](https://user-images.githubusercontent.com/93143005/181093018-ada9bbc8-8300-4f34-b390-700565ac3d97.png)
file:///home/hp/Pictures/Screenshot%20from%202022-07-27%2000-45-40.png![image](https://user-images.githubusercontent.com/93143005/181093048-b31c8af2-528a-4a1e-8ec3-b4129a548348.png)
file:///home/hp/Pictures/Screenshot%20from%202022-07-27%2000-45-50.png![image](https://user-images.githubusercontent.com/93143005/181093074-8d172525-fc05-41a4-bd52-cc0925335fad.png)
file:///home/hp/Pictures/Screenshot%20from%202022-07-27%2000-45-58.png![image](https://user-images.githubusercontent.com/93143005/181093115-f59142da-6473-42f8-b6e4-00d80bce21fd.png)

##Conclusion
We can infer from the outcomes that deep learning is one of most accurate approach for autonomous vehicles
Therefore we believe that future projects will profit incredibly from presenting a framework that uses the merits of other techniques with the computational potential of CNN model

## Future-work
Add other features such as break and acceleration 
More training data with different scenarios (such as increasing and decreasing light conditions in images) so that our model could be more robust
Implementing the CNN in the physical car could have the great impact on accuracy of the model
Also, we can use hybrid model (CNN and RNN etc.) accuracy should be increased significantly.





# Dataset 
https://github.com/SullyChen/driving-datasets
