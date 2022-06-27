# Graceful Degradation
Authors: Shalini Chaudhuri, Joseph Miano, Santyblesson Pushparaj, Sreehari Sreejith

## Notes
Link to YouTube video going over the demo notebook: https://youtu.be/NoV8i8zvGi8

Experiments to understand degradation in neural networks 

Dataset used for image models: https://www.kaggle.com/ajayrana/hymenoptera-data 
Note on the dataset used: Our initial plan was to use the well-known CIFAR 10 dataset. But with some initial experiments, we found that using the 32x32 images from CIFAR 10 would not allow us to use the power of pretrained models such as AlexNet to the full extent (due to the need to resize images to 224x224 for such models). We knew that writing our own convnet was possible, but it would mean training the network for a longer period of time to get to similar levels of accuracy for our baseline model. Hence the choice to use AlexNet in a transfer learning setting which allows us to work with a nice, small dataset for fast experimentation yet with reasonable accuracies. 

References used for Image models:

Transfer Learning: https://pytorch.org/tutorials/beginner/transfer_learning_tutorial.html 

Pruning: https://pytorch.org/tutorials/intermediate/pruning_tutorial.html 


Dataset used for audio models: https://urbansounddataset.weebly.com/urbansound8k.html


