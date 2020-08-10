# Multi Task Learning 

The aim of multi task learning is to leverage two (or more) related tasks in the learning process with the hope that leanring one task aids perfromance in learning the other task(s) and thus improves predicitve power for at least one (ideally all) of the tasks. 

There are two distinct flavours of MTL: Hard parameter sharing and soft parameter sharing. In this project, the former is investigated.
Hard paramter sharing invloves two tasks sharing a common network which splits into task specific paths (e.g. a series of convolutional layers with two paths of dense layers for two seperate tasks). 

This project uses the FASHION MNIST dataset to compare MTL against individual task networks. The two tasks in question are:
- Task 1 - Clothing item 10 class classification (e.g. shoes, t-shirts etc) across 10 classes
- Task 2 - Clothing category classification - predicitng whether a viewed clothing image belongs to one of three groups. These groups are shoes (Sandal, Sneaker and Ankle Boot),  Gendered (Dress, Shirt and Bag) and Uni-Sex (T-shirt, Trouser, Pullover and Coat). 

## Results

Experiments demonstrate that Multi Task Learning is able to improve both training and test accuracy and reduce loss for both tasks 1 and 2.

![test](https://github.com/JSaunders97/multi-task-learning/blob/master/Q6_2_MTL_Test_Accuracy.png)

![train](https://github.com/JSaunders97/multi-task-learning/blob/master/Q6_MTL_Training_Accuracy.png)

![loss](https://github.com/JSaunders97/multi-task-learning/blob/master/Q6_MTL_Network_Loss.png)
