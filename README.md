# Project: Generating Blood Cell Images

Implementation and comparison of three generative approaches, a Variational AutoEncoder, a Generative Adversarial Network, and a Denoising Diffusion Probabilistic Model, trained to generate images of blood cells across 8 cell classes.

## Workflow
1. Balance the dataset by upsampling minority classes to match the majority class.
2. Normalize and resize all images for consistent model input.
3. Train the VAE, GAN, and DDPM independently using matching hyperparameters where possible.
4. Generate sample images from each model and compare them visually against real images.
5. Score generation quality using Fréchet Inception Distance where computation was feasible.

## Results
Image quality was measured with Fréchet Inception Distance, lower is better, averaged over 5 runs. The VAE scored 187.86, the GAN scored 83.02. The DDPM could not be scored due to generation time, but produced the sharpest and most detailed images among the three, suggesting it could outperform the GAN with proper quantitative evaluation.

## Technologies
Python, PyTorch, NumPy, Jupyter Notebook.

## Contents
* `project.ipynb` notebook with the project code
* `report.pdf` project report
