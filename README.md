# Neural Network for Image Fitting and Neural Radiance Fields (NeRF)

This repository contains a project focused on using neural networks for image fitting and implementing a Neural Radiance Field (NeRF) for rendering 3D scenes.

## Project Overview
The project is divided into two main tasks:

### Part 1: Fitting a 2D Image
- **Positional Encoding:** Implemented sinusoidal positional encoding to map pixel coordinates into a higher-dimensional space.
- **MLP Design:** Designed a Multi-Layer Perceptron (MLP) with three layers for color prediction.
- **Image Fitting:** Trained the MLP on a 2D image using pixel-wise regression and evaluated using Peak Signal-to-Noise Ratio (PSNR).

### Part 2: Fitting a 3D Scene (NeRF Implementation)
- **Ray Calculation:** Computed ray origins and directions using intrinsic and extrinsic camera parameters.
- **Ray Sampling:** Sampled points along each ray for volume rendering.
- **NeRF MLP Design:** Implemented a NeRF model using a 10-layer MLP with ReLU and Sigmoid activations for density and color prediction.
- **Volume Rendering:** Applied volumetric rendering techniques for realistic scene generation.
- **Training Pipeline:** Trained the NeRF model to generate novel views of a 3D scene.

## Requirements
- Python 3.x
- PyTorch
- NumPy
- Matplotlib

## Files
- `neural_rendering.py`: script containing all code.
- '*.pt': model weights

## Usage
1. Clone this repository.
2. Install the required packages using `pip install -r requirements.txt`.
3. Run the script `neural_rendering.py`.

## Results
- Achieved high PSNR scores for both 2D image fitting and NeRF training.
- Successfully rendered novel views of a 3D scene using the NeRF model.
