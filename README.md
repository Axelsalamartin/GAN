# Generative Adversarial Networks (GAN) :

Generative Adversarial Networks are used in a lot of ways. They're a lot of different variations of it such as DiscoGAN, pix2pix and many others. 

The main goal in this exemple will be to create new images of handwritten digits. For that we will train the model on the MNIST dataset. 

PS : To keep samples from training and vizualize them, create a directory called "GAN" one level higher than the notebook or change the path inside the code

## But how does it works ?

The concept of GAN is to train two model together so that they benefit from each other's progress :

 - A Generator
 - a Discriminator
 
The Generator will generate outputs and the discriminator will judge it by comparing it to the real data we provide. So here we will give the discriminator images of handwritten digits and it'll tell the generator if the images it creates are close to real ones or not. 

To make it short :
During the training the generator will learn to generate output really close to the original dataset and the discriminator will become better at differenciating real one from fake one. In the end the generator's outputs start to look really close to the image we provide so it means we can create new images to get new variations of the original dataset.

