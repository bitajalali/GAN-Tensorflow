# Tensorflow-GAN
This model includes two generative and discriminator structures, the way it works is as follows:
We give a noise vector with size 100 as input to the model Then, the generator part creates a fake 
image by deconvolution operation, and then there is the discriminator model, which has the task 
of distinguishing between the fake image fed by the generator and the original images, this structure
is done by a function using the gradient tape tool as follows: The data goes to the generator, and its output
goes to the discriminator, and the discriminator is trained one step. in this model we use Cross-Entropy loss function.
in the following, we show the structure of the model and a few samples of images that the GAN model produced:
## generative model:
![G](https://user-images.githubusercontent.com/115353236/199777145-3392b007-4538-415d-bfca-ffcb83760bc4.PNG)


## discriminator model:
![d](https://user-images.githubusercontent.com/115353236/199777185-8731f469-6508-42c7-bd54-503b8b360cd3.PNG)
### output in epoch 150:
![150](https://user-images.githubusercontent.com/115353236/199779061-b7bee046-0d8c-4753-b3ca-311ea78b5c72.PNG)
### output in epoch 199:
![199](https://user-images.githubusercontent.com/115353236/199779122-44ace2b3-23fe-470b-9e21-135c629f52c3.PNG)
### output in epoch 200:
![200](https://user-images.githubusercontent.com/115353236/199779185-ec8d2a53-049d-4c1c-8cee-05b49e9af083.PNG)
