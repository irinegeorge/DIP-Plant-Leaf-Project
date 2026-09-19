# Restoration and Segmentation of Diseased Regions in Plant Leaf Images Using Digital Image Processing

## Project Overview
This project applies classical Digital Image Processing techniques to restore, enhance, detect edges, segment, and evaluate diseased regions in plant leaf images.

The project uses corresponding ground-truth masks for quantitative segmentation evaluation.

## Objectives
- Add Gaussian noise to simulate image degradation.
- Restore noisy images using mean and median filtering.
- Evaluate restoration using MSE, PSNR, and SSIM.
- Improve image contrast using histogram equalization.
- Perform global thresholding, Otsu thresholding, and adaptive thresholding.
- Detect image boundaries using Sobel and Canny edge detection.
- Refine segmentation using morphological opening and closing.
- Apply Watershed segmentation with foreground/background markers.
- Compare the predicted segmentation with the ground-truth mask.
- Calculate IoU, Dice coefficient, and segmentation accuracy.

## Dataset
The notebook expects a ZIP dataset named `leaf.zip` with this structure:

```text
leaf/
├── image/
└── masks/
```

Each image should have a corresponding mask with the same base filename.

## Technologies
- Python
- OpenCV
- NumPy
- Matplotlib
- scikit-image
- Google Colab / Jupyter Notebook

## Project Pipeline
Original Leaf Image
→ Grayscale Conversion
→ Gaussian Noise
→ Mean/Median Restoration
→ MSE/PSNR/SSIM
→ Histogram Equalization
→ Thresholding
→ Sobel + Canny
→ Morphological Processing
→ Watershed Segmentation
→ Ground Truth Comparison
→ IoU + Dice + Accuracy

## Files
- `dipprojectnew.ipynb` — complete interactive notebook
- `source_code.py` — Python source extracted from notebook code cells
- `requirements.txt` — required Python packages
- `report/` — project report
- `images/` — project input/output images if required
- `screenshots/` — screenshots of important results

## How to Run
1. Open `dipprojectnew.ipynb` in Google Colab.
2. Upload the required `leaf.zip` dataset when prompted.
3. Run the cells from top to bottom.
4. Save important output figures/screenshots into `screenshots/`.
5. Add the final project report to `report/`.

## Evaluation Metrics

### Restoration
- Mean Squared Error (MSE)
- Peak Signal-to-Noise Ratio (PSNR)
- Structural Similarity Index (SSIM)

### Segmentation
- Intersection over Union (IoU)
- Dice Coefficient
- Accuracy
