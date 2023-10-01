# GANs_models
Wasserstein GANs architectures CIFAR10

WGAN algorithm implemented with gradient penalty architecture.

![image](https://github.com/moriyatur/GANs_models/assets/142314356/3d296c13-282c-4a21-8429-da39a591343b)

WGAN with GP is implemented by using the Wasserstein distance as the loss function in the WGAN framework, along with a gradient penalty term added to the discriminator's loss to enforce the Lipschitz constraint and improve stability during training.

The gradient penalty encourages the gradient of the discriminator's output with respect to the input samples to have a norm of 1. This penalty term helps to prevent the discriminator from becoming too powerful and improves training stability. The gradient penalty is typically calculated using the L2 norm of the gradients and added to the discriminator's loss.

The loss function as a function of the iterations for training with the DCGAN and the WGAN :
![image](https://github.com/moriyatur/GANs_models/assets/142314356/488320b7-5f8d-4a40-90eb-3b3e19a03da6)

A set of real images and their classification for comparison with the two popular variants of the generative adversarial network (GAN) architecture:

# Generated fake images during the training process after a number of epochs of training.
We can see that the success of convergence in GAN training can depend on various factors, such as the specific dataset, architecture choices, hyperparameters, and training procedures.
The number of failed convergences can vary greatly based on these factors and the specific implementation details.
When we experimented with different strategies, many iterations on the training process and hyperparameter changes, we could eventually lead to successful convergences in the GAN training of the models.

WGAN_GP

![image](https://github.com/moriyatur/GANs_models/assets/142314356/174a57b7-f604-4f6e-992b-1b3014a18d1c)
![image](https://github.com/moriyatur/GANs_models/assets/142314356/51233ae8-eb31-488c-8e94-afe37e7f211f)
![image](https://github.com/moriyatur/GANs_models/assets/142314356/c2e867f8-1683-4ab4-aebc-a2c3a96c7bc2)


DCGAN

![image](https://github.com/moriyatur/GANs_models/assets/142314356/50bba35b-6c63-43b0-b572-ceceb2876774)
![image](https://github.com/moriyatur/GANs_models/assets/142314356/708af96d-ca8f-4348-b8b1-867442cb9460)
![image](https://github.com/moriyatur/GANs_models/assets/142314356/712968a5-6d6d-43a9-a13a-d0a75afe2f11)


Each of the GANs architecture (DCGAN and WGAN_GP) consists of generator, discriminator and training functions separately. We train the models with the Adam optimizer with the same hyperparameters for both models (learning rate and betas).
