# mittal-24-FFHQ-DDPM-Diffusion-Model 
This link is for downloading dataset
https://drive.google.com/drive/folders/1LeEaAy7Bc66tmabL5CsYYBqjVBoJ3NGW?usp=drive_link
# FFHQ Face Image Generation using DDPM

## Project Overview

This project implements a Denoising Diffusion Probabilistic Model (DDPM) to generate face images using the FFHQ (Flickr-Faces-HQ) dataset.

The model learns the process of gradually adding noise to images and then reversing this process to generate new images from random noise.

The project uses a small subset of 100 FFHQ images resized to 64×64 pixels for experimental training.

## Objectives

- Understand the working of diffusion models.
- Implement the forward diffusion process.
- Build a U-Net-based noise prediction model.
- Train the model using a noise prediction objective.
- Implement the reverse diffusion process.
- Generate new images from random noise.

## Technologies Used

- Python
- PyTorch
- Google Colab
- NumPy
- Matplotlib
- FFHQ Dataset

## Model Architecture

The project uses a DDPM architecture with a U-Net-based neural network.

**Main components:**

1. Forward Diffusion: Gradually adds Gaussian noise to input images.
2. Noise Prediction: U-Net learns to predict the noise added to an image.
3. Training: The model is trained using Mean Squared Error (MSE) loss.
4. Reverse Diffusion: The learned model progressively removes noise to generate images.

## Dataset

- Dataset: FFHQ (Flickr-Faces-HQ)
- Images used: 100
- Image format: RGB
- Training image size: 64×64
- Normalization: [-1, 1]

The dataset is not included in this repository. Users must obtain the dataset separately and configure the dataset path before running the notebook.

## Training Configuration

- Diffusion timesteps: 1000
- Optimizer: Adam
- Learning rate: 0.0001
- Loss function: Mean Squared Error (MSE)
- Training images: 100

## How to Run

1. Clone this repository.
2. Open the notebook in Google Colab.
3. Obtain the FFHQ dataset and upload the ZIP file to Google Drive.
4. Update the dataset path in the notebook.
5. Run the notebook cells in order.
6. Train the model and generate images.

## Project Structure

```text
FFHQ-DDPM-Diffusion-Model/
│
├── DDPM_FFHQ.ipynb
├── README.md
├── requirements.txt
└── outputs/
```

## Results

The model was trained experimentally on 100 images. The generated outputs and training loss are used to evaluate the learning process.

Due to the limited dataset size and training duration, generated images may contain noise or blurry features. This is an experimental implementation and not a production-ready face generation model.

## Future Improvements

- Train on a larger dataset.
- Increase the number of training epochs.
- Improve the U-Net architecture.DESC
- Experiment with different image resolutions.
- Evaluate generated image quality using suitable metrics.

## Author

BTech Computer Science and Engineering Student

## Acknowledgement

This project is developed for academic learning and experimentation with Denoising Diffusion Probabilistic Models (DDPM).
