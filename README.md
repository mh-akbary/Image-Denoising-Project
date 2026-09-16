# Image Denoising Project

A comparative study of image denoising techniques using different noise models and spatial filtering methods.

## Overview

This project investigates the performance of different spatial filters for removing various types of noise from grayscale images.

The main objective is to evaluate and compare denoising filters under different noise conditions using quantitative image-quality metrics and visual comparisons.

The experiments were performed on a dataset of **300 grayscale images**.

## Dataset

The experiments were conducted using a dataset containing **300 grayscale images**.

For each noise type, noisy versions of the images were processed using multiple spatial filtering methods. The filtered results were then compared with the corresponding original images.

## Noise Types

Seven different noise types were investigated:

1. Gaussian Noise
2. Salt and Pepper Noise
3. Poisson Noise
4. JPEG Noise
5. Speckle Noise
6. Multiplicative Noise
7. Quantization Noise

## Denoising Filters

Four spatial filtering techniques were evaluated:

- **Mean Filter**
- **Gaussian Filter**
- **Median Filter**
- **Bilateral Filter**

Different kernel sizes were tested:

- 3×3
- 5×5
- 7×7

## Evaluation Metrics

The performance of the denoising methods was evaluated using three image-quality metrics.

### Mean Squared Error (MSE)

MSE measures the average squared difference between the original image and the filtered image.

**Lower MSE indicates lower reconstruction error.**

### Peak Signal-to-Noise Ratio (PSNR)

PSNR measures the similarity between the original and reconstructed images.

**Higher PSNR generally indicates better reconstruction quality.**

### Structural Similarity Index (SSIM)

SSIM measures structural similarity between the original and filtered images.

Values closer to 1 indicate greater structural similarity.

## Experimental Procedure

The project follows the following workflow:

1. Load the grayscale image dataset.
2. Generate and/or load images containing different noise types.
3. Visualize the original image and its noisy versions.
4. Select test images for visual analysis.
5. Apply the Mean, Gaussian, Median, and Bilateral filters.
6. Test different filter kernel sizes.
7. Calculate MSE, PSNR, and SSIM for the filtered images.
8. Evaluate the filters across all 300 images.
9. Calculate the average performance of each filter.
10. Generate comparison tables and visualization charts.
11. Compare filter performance across all seven noise types.

## Results

The results were evaluated separately for each noise type.

The results include:

- Average MSE
- Average PSNR
- Average SSIM
- Visual comparisons of original, noisy, and filtered images
- Filter performance comparison tables
- Bar charts for MSE, PSNR, and SSIM

## Visual Analysis

The project includes visual comparisons showing:

- Original images
- Noisy images
- Filtered images

These visualizations provide a qualitative comparison of how each filtering method affects image noise, details, and structures.

## Quantitative Analysis

The quantitative evaluation is based on the average results obtained from the complete dataset.

| Metric | Interpretation | Desired Direction |
|--------|----------------|-------------------|
| MSE | Reconstruction error | Lower |
| PSNR | Reconstruction quality | Higher |
| SSIM | Structural similarity | Higher |

## Final Comparison

A final comparison was performed across all seven noise types.

The comparison considers:

- MSE
- PSNR
- SSIM

The purpose of this comparison is to examine how filter performance changes depending on the type of noise and the filter configuration.

The results demonstrate that the effectiveness of a denoising filter depends on the characteristics of the noise, the selected filter, and the kernel size.

## Technologies

The project was implemented in Python using:

- Python
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
├── image-denoising-filter-comparison-and-evaluation.ipynb
├── README.md
├── requirements.txt
├── .gitignore
└── ...
```
گگگ

## Conclusion

This project provides a comparative evaluation of spatial image denoising filters under seven different noise conditions.

The experiments show that denoising performance varies depending on:

- The type of noise
- The selected filtering method
- The filter kernel size
- The evaluation metric

The combination of visual analysis and quantitative metrics provides a comprehensive evaluation of the investigated denoising methods.

## Author

**Mohadese Akbary**

GitHub: @mh-akbary
