# Incption-Resnet
Classification of Breast Cancer using Histopathological Images

### Overview
Classifying histopathological breast cancer images using convolution neural networks. 
In addition to identifying malignancy or benignity, the model classifies the sub-class of the image. 

### Modules
<ol>
<li> Data Augmentation </li>
In the real world, a target application may exist in a variety of conditions, such as different orientation, location, scale, brightness etc.
This is accounted for by training the neural network with additional synthetically modified data. 
This modification is done by scaling, translation rotation (at 90 degrees), flipping and adding noise.

<li> Training </li>
Training is done by using the following two models:
  <li> Inception v3 </li>
  <li> Inception-Resnet-v2 </li>
  The networks are pre-trained using ImageNet and flowers dataset. Transfer learning will be adopted for training on the chosen dataset.
In transfer learning, the knowledge of an already trained Machine Learning model is applied to a different but related problem.
The weights that a Network has learned at Task A are transferred to a new Task B. It saves training time and gives a better performance. 

<li> Validation </li>
The augmented dataset is randomly split into 70% for training, 15% for validation and 15% for testing. The performance metric used is accuracy.

<li> Hyperparameter Tuning </li>
Hyperparameters directly control the behaviour of the training algorithm. They have a significant impact on the performance of the model.
The hyperparameters of tuned here are learning rate, number of epochs, activation function and number of hidden layers in order to give better performance. 
Tuning is done based on validation performance, and finally tested on the test set.

</ol>

