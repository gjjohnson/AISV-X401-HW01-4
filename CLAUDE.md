# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Project Context

This is a directory for the 
**AISV.X401 (Deep Learning and Artificial Intelligence)**  course. 

Topics: Color Histogram + HOG

Instructions: Use NumPy for all numeric computation. Do not use PyTorch/TensorFlow/JAX. You may use
scikit-image only where explicitly allowed (HOG, optional image loading).

Allowed libraries:
 numpy (required)
 matplotlib (optional, for debugging/plots)
 scikit-image (allowed only for HOG and optional image I/O: skimage.io.imread)

Not allowed:
 Deep learning frameworks: PyTorch, TensorFlow, JAX, Keras
 Auto-diff packages for gradients (you must derive/implement gradients manually)
 High-level ML libraries for these tasks (e.g., sklearn KNN/softmax classifiers)


## Notes

### Notebooks
- `GJJohnsonAISV0401HW01_4.ipynb` — Image Features: Color Histogram + HOG. Create notebook to be run in Google Colab.

### Dependencies
```
numpy
matplotlib
```
No `pip install` required beyond a standard Python environment (both are included in Colab by default).

### Running the Notebook
1. Open `GJJohnsonAISV0401HW01_4.ipynb` in Colab or locally with `jupyter notebook`.
2. Run all cells top-to-bottom (`Runtime → Run all` in Colab).

### Model Architecture / Data Pipeline
Implement two global image feature extractors for RGB images: 
(a) per-channel color histogram (e.g., 16 bins per channel) concatenated; 
(b) HOG descriptor on the grayscale image. 

Given a list of RGB images, return X_feat (N×F). Use scikit-image for HOG only; implement histograms using NumPy



