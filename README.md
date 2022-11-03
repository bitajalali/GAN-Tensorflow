# Tensorflow-GAN
This model includes two generative and discriminator structures, the way it works is as follows:
We give a noise vector with size 100 as input to the model Then, the generator part creates a fake 
image by deconvolution operation, and then there is the discriminator model, which has the task 
of distinguishing between the fake image fed by the generator and the original images, this structure
is done by a function using the gradient tape tool as follows: The data goes to the generator, and its output
goes to the discriminator, and the discriminator is trained one step. in this model we use Cross-Entropy loss function.
