# AI Declaration - Task 1: Variational Auto-encoders

## AI Tools Used
- Claude (Anthropic)

## Prompts Used

1. Build a VAE in PyTorch for 256×256 grayscale brain MRI images with 4-layer encoder/decoder, 2D latent space, and KL divergence loss.

2. Write code to check GPU availability, set device (CUDA/CPU), and print device specs.

3. Write code to load OASIS brain MRI PNG images with data augmentation and create DataLoaders (batch_size=16).

4. Write code to build VAE encoder (conv layers → 2D latent), reparameterization trick, decoder (transpose conv), and VAE loss (BCE + KL).

5. Write code to set up Adam optimizer (lr=0.001) and training configuration.

6. Write train_epoch() and test_epoch() functions with loss computation for VAE.

7. Write code to generate brain images from 5×5 latent space grid.

8. Write code to download files from Google Colab to local machine.