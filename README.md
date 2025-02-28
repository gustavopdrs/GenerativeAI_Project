Generative Adversarial Network (GAN) Implementation for MNIST. 

This project demonstrates a PyTorch-based implementation of a Generative Adversarial Network (GAN) to generate realistic MNIST-like images. The code includes the creation and testing of generator and discriminator models, loss functions, and the training loop.

Features
1. Generator:
The generator creates fake MNIST-like images using a noise vector as input.

Key Components:
Fully connected layers with batch normalization and ReLU activation.
Final layer with a sigmoid activation for output image generation.
Defined Classes and Functions:
get_generator_block(input_dim, output_dim)
Generator(z_dim, im_dim, hidden_dim)

2. Discriminator:
The discriminator classifies whether an image is real (from the dataset) or fake (generated by the generator).

Key Components:
Fully connected layers with LeakyReLU activation.
Final linear layer for real/fake prediction.
Defined Classes and Functions:
get_discriminator_block(input_dim, output_dim)
Discriminator(im_dim, hidden_dim)
3. Loss Functions
Custom functions for generator and discriminator losses using Binary Cross Entropy Loss:

get_gen_loss for generator loss.
get_disc_loss for discriminator loss.

4. Noise Generation:
Function get_noise generates random noise vectors as input for the generator.

5. Training Loop:
The code includes a comprehensive training loop:

Updates discriminator and generator weights.
Tracks and displays generator and discriminator losses.
Visualizes real and generated images at regular intervals.

------------------------------------------------------------
Requirements:
- Python 3.7 or higher
- PyTorch 1.7.0 or higher
- torchvision
- tqdm
- matplotlib


License
This project is licensed under the MIT License. See the LICENSE file for details.
