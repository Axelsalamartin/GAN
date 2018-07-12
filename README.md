# Generative Adversarial Network (GAN) :

Generative Adversarial Network are used in a lot of ways. They're a lot of different variations of it such as DiscoGAN, pix2pix and many others. 

The main goal in this exemple will be to create new images of handwritten digits. For that we will train the model on the MNIST dataset. 

PS : to keep the samples and vizualize create a directory called "GAN" one level higher than the notebook or change the path inside the code

## But how does it works ?

The concept of GAN is to train two model together so that they benefit from each other's progress :

 - A Generator
 - a Discriminator
 
The Generator will generate output and the discriminator will judge it by comparing it to the real data we provide. So here we will give the discriminator images of handwritten digits and it'll tell the generator if the image it creates is close to a real one or not. 

On the beginning both of them will be bad at their jobs. The generator will give output that won't look like anything at all and the discriminator won't be able to differenciate real image from fake one. But we provide real image to the discriminator so it will get better and start telling the generator that it's work is bad so it'll update his output to get better. By becoming better the discriminator's task will get more difficult and it'll have to progress to still be able to differenciate the real one and the others. 

To make it short :
During the training the generator will learn to generate output really close to the original dataset and the discriminator will become better at differenciating real one from fake one. In the end the generator' output become to look really close to the image we provide so it means we can create new image to get new variations of the original dataset.

