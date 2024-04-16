##  RESNET CIFAR-10 : TEAM KSS 🐍
Welcome to our project to train and test oN CIFAR-10 data with around 4.5 Million parameters usign Residual networks and modifications on it!

#### Steps to reproduce results :

1. Using  google colab : 
    - Connect to colab
    - Upload the folder provided "deep-learning-mini-project-spring-24-nyu" to drive
    - Mount google drive to colab
    - Run all cells

OR 

2. Locally : 
    - Replace the path in cell 6 to replace the ```batch = "" ```to contain the folder which has all training files.
    - and ```test_file =""``` to location of file to 'cifar_test_nolabels.pkl' 

#### Notes : 
The code runs for about 40-50 mins on GPU. We have prioritized faster training in our models to experiment with multiple parameters. We play around with density of the network, data augementation, lr scheduler, dropout layers to see impact! 

At the end of training it produces a checkpoint that can be used later to test and validate the model.We have included testing and validation in the code later after training ourselves which can be used as well. 

The best results can be achieved with : 
-  channels : ```channels = [32, 64, 256, 256]```
-  lr_scheduler : *In Cell 15*, #Optimizer part, we can uncomment the scheduler part to enable lr_scheduler and *Cell 18* to to uncomment the scheduler.step()
- Dropout layer is set to 2
- Dropout probablity is set to 0.2


Hope you have fun playing around with parameters and navigating the code :) 

