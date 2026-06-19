# MNIST Autoencoder 
This project implements a fully connected autoencoder in PyTorch trained on the MNIST handwritten digit dataset.

## Objective

To investigate whether meaningful features can be learnt without supervision by compressing handwritten digit images into a two-dimensional latent space.

## Model Architecture

784 → 128 → 64 → 2 → 64 → 128 → 784

- Optimiser: Adam
- Learning Rate: 0.001
- Loss Function: Mean Squared Error (MSE)
- Epochs: 12
- Batch Size: 64

## Results

- Final Test Loss: 0.0386
- Distinct digit clusters emerged in latent space despite no label supervision.
- Similar digits such as 4 and 9 showed overlap in latent space.
- Strong dimensional compression produced recognisable reconstructions but introduced some blurring.

