# DC-GAN

It is Generative Adversial Network model proposed by Alec Radford & Luke Metz in 2016. DCGAN uses convolutional and convolutional-transpose layers in the generator and discriminator, respectively.

## Architecture guidelines for stable Deep Convolutional GANs

• Replace any pooling layers with strided convolutions (discriminator) and fractional-strided convolutions (generator).

• Use batchnorm in both the generator and the discriminator.

• Remove fully connected hidden layers for deeper architectures.

• Use ReLU activation in generator for all layers except for the output, which uses Tanh.

• Use LeakyReLU activation in the discriminator for all layers.

[Research paper](https://arxiv.org/pdf/1511.06434.pdf) for more reference.