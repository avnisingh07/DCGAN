# DCGAN for Face Generation using CELEBA Dataset

## Introduction

This project utilizes a Deep Convolutional Generative Adversarial Network (DCGAN) to generate lifelike face images from the CELEBA dataset. The model, built with PyTorch, comprises a generator and a discriminator that are trained adversarially.

---

## Dataset Preprocessing Steps

- Obtain the **CELEBA dataset** from [Kaggle](https://www.kaggle.com/datasets).
- Resize and standardize images to a **64x64** resolution.
- Transform images into **tensors** and scale pixel values to the range **[-1, 1]**.
- Utilize **PyTorch's DataLoader** for efficient batch loading.

---

## Training the Model

1. Set hyperparameters:
   - Batch size
   - Learning rate
   - Number of epochs

2. Initialize:
   - Generator network
   - Discriminator network

3. Define:
   - Loss functions
   - Optimizers

4. Train the model:
   - Train the **discriminator** to distinguish real and fake images.
   - Train the **generator** to produce realistic images that can fool the discriminator.

5. Save progress:
   - Generator: `generator.pth`
   - Discriminator: `discriminator.pth`
   - Generate and save output images after each epoch.

---

## Testing the Model

- Load the trained **generator** model.
- Generate new face images using **random noise** as input.
- Save and visualize the generated outputs.

---

## Expected Outputs

- **Generated Images**: Over time, the model will produce increasingly realistic human faces.
- **Loss Curves**: Both generator and discriminator losses will decrease and stabilize.

---

## Example Outputs

- **Generated Face**:  
  *(Include a sample output image here)*

- **Loss Curve**:  
  *(Insert generator and discriminator loss graph here)*

---

## Requirements

- Python 3.x  
- PyTorch  
- torchvision  
- Matplotlib  
- PIL  
- Kaggle API (for dataset download)
