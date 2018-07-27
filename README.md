# Generative Adversarial Networks (GAN) :

Generative Adversarial Networks are used in many tasks such as style transfert or new image generation.

The main goal in this exemple will be to create new images of handwritten digits. For that we will train the model on the MNIST dataset. 

## But how does it works ?

The concept of GAN is to train two model together so that they benefit from each other's progress :

 - A Generator
 - a Discriminator

To make it short :
During the training the generator will learn to generate output really close to the original dataset and the discriminator will become better at differenciating real one from fake one. In the end the generator's outputs start to look really close to the images we provide so it means we can create new images to get new variations of the original dataset.


PS : To keep samples from training and vizualize them, create a directory called "GAN" one level higher than the notebook or change the path inside the code.

