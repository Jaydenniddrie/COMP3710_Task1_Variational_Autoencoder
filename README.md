# Task 1: Variational Autoencoder (VAE) on OASIS Brain MRI

## Overview
Trained a 2D latent space VAE to compress and generate brain MRI images from the OASIS dataset.

## Dataset
- **Source:** OASIS Brain MRI (keras_png_slices_data)
- **Images:** 544 grayscale PNG slices (256×256)
- **Task:** Learn latent representation of brain anatomy

## Model
- **Type:** Variational Autoencoder (VAE)
- **Encoder:** 4 conv layers (1→32→64→128→256 channels) → 2D latent space
- **Decoder:** 4 transpose conv layers (256→128→64→32→1 channels)
- **Loss:** Reconstruction (BCE) + KL divergence
- **Optimizer:** Adam (lr=0.001)

## Results
- **Training Epochs:** 50
- **Dataset Size:** 544 images
- **Final Loss:** 8818.25
- **Hardware:** Google Colab GPU (T4)
- **Training Time:** ~5-10 minutes

## Visualizations
1. **latent_manifold.png** - 2D scatter of all 544 images in latent space
2. **generated_brains.png** - 5×5 grid of VAE-generated brain images from latent space

## Files
- `task1_vae.ipynb` - Complete training notebook (run on Google Colab)
- `ai_declaration.md` - AI prompts and usage disclosure
- `results/` - Trained model, loss metrics, visualizations

## How to Run
1. Upload `task1_vae.ipynb` to Google Colab
2. Upload `keras_png_slices_data.zip` to Colab
3. Run all cells
4. Download results to `results/` folder