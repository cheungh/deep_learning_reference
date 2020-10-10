## TensorFlow Official StyleGAN repository from GitHub
- !git clone https://github.com/NVlabs/stylegan.git

## Concept
- generator and discriminator 
- noise vectors fed to the generator
- truncation
- batch normalization (help better performance and smooth out)

## Common Activation Functions
### ReLU 
 - watch out for Dying ReLU problem. Once reaches zero will still zero
 - When z <= 0,  the derivative equals zero, causing some neurons to get stuck and stop learning.
### Leaky ReLU 
Improvement on Dying ReLU problem, allow small leak for negative value, and have a slope below zero
### Sigmoid 
- y between (0 to 1) 
- Not used in hidden layer(s)
- with vanishing gradient problems where saturated outputs occur at the tails of the function
### Tanh
- y between (-1 to 1)
- Not used in hidden layer(s)
- with vanishing gradient problems where saturated outputs occur at the tails of the function
