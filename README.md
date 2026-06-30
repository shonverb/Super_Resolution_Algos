# Deep Learning Image Super-Resolution Benchmark

This repository provides a comprehensive benchmarking suite for Image Super-Resolution algorithms. It compares traditional interpolation methods against Deep Learning models using standard metrics.

**Note:** This script is optimized to run as a standalone environment in Google Colab.

## 🚀 Features
* **Models Evaluated:** Compares Bicubic interpolation, SRCNN (Super-Resolution Convolutional Neural Network), and ESRGAN (Enhanced SRGAN).
* **Automated Datasets:** Automatically fetches standard HR/LR datasets (Set5/Set14).
* **Dynamic Training:** Includes a fallback mechanism to train the SRCNN model from scratch using the T91 dataset if pre-trained weights are unavailable.
* **Metrics:** Evaluates outputs using Peak Signal-to-Noise Ratio (PSNR) and Structural Similarity Index (SSIM) on the Y-channel (shaved borders).

## 🛠️ Usage
1. Open [Google Colab](https://colab.research.google.com/).
2. Upload the `super_resolution_benchmark.py` (or `.ipynb`) file.
3. Select a GPU Runtime (`Runtime` -> `Change runtime type` -> `T4 GPU`).
4. Run all cells. The script will automatically handle dependencies, weights downloading, and testing.
