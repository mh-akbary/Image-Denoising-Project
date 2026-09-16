# Image Denoising Project

## Overview

This project investigates image denoising using different noise models and spatial filtering methods.

The main objective is to compare the performance of several denoising filters under different types of image noise.

## Dataset

The experiments were performed on a dataset containing 300 grayscale images.

For each noise type, the noisy images were processed using several spatial filtering methods.

## Noise Types

The following seven noise types were investigated:

- Gaussian Noise
- Salt and Pepper Noise
- Poisson Noise
- JPEG Noise
- Speckle Noise
- Multiplicative Noise
- Quantization Noise

## Denoising Filters

Four spatial filters were evaluated:

- Mean Filter
- Gaussian Filter
- Median Filter
- Bilateral Filter

For most filters, different kernel sizes were tested:

- 3×3
- 5×5
- 7×7

## Evaluation Metrics

The performance of the filters was evaluated using three image quality metrics:

### MSE

Mean Squared Error (MSE) measures the average squared difference between the original and filtered images.

Lower MSE indicates a smaller reconstruction error.

### PSNR

Peak Signal-to-Noise Ratio (PSNR) measures the quality of the reconstructed image.

Higher PSNR generally indicates better image quality.

### SSIM

Structural Similarity Index (SSIM) measures the structural similarity between the original and filtered images.

Values closer to 1 indicate greater structural similarity.

## Experimental Procedure

The experiment follows these main steps:

1. Load the image dataset.
2. Visualize different noise types.
3. Select test images.
4. Apply different denoising filters.
5. Evaluate the filtered images using MSE, PSNR, and SSIM.
6. Rank the filters based on their performance.
7. Evaluate the filters on all 300 images.
8. Calculate the average performance for each filter.
9. Compare the results for all noise types.

## Results

The performance of the filters was compared separately for each noise type.

The results include:

- Average MSE
- Average PSNR
- Average SSIM
- Visual comparisons of original, noisy, and filtered images
- Comparison charts for the evaluated filters

## Final Comparison

A final comparison was performed to examine filter performance across the seven noise types.

The comparison focuses on the three evaluation metrics:

- MSE
- PSNR
- SSIM

## Technologies

The project was implemented using Python and the following libraries:

- OpenCV
- NumPy
- Pandas
- Matplotlib
- scikit-image
- Jupyter Notebook

## Project Structure

```text
Image-Denoising-Project/
│
├── Image_Denoising.ipynb
├── README.md
└── ...

## Conclusion

This project provides a comparative evaluation of different spatial denoising filters under multiple noise conditions.

The experimental results demonstrate that filter performance depends on the type of noise and the filter configuration.
