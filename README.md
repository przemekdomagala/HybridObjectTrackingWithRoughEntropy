# Hybrid Object Tracking with Rough Entropy

![Tracking Pipeline](tracking_pipeline.png)

This project implements a hybrid object tracking pipeline that integrates Rough Entropy concepts with traditional change detection methods for improved accuracy in satellite image sequences. Project utilizes data from [Change Detection 2014 dataset](https://www.kaggle.com/code/kerneler/starter-change-detection-2014-042f59d1-1/input).

## 📁 Dataset

We use the **Change Detection 2014** dataset which contains before-and-after satellite imagery, ideal for evaluating change and movement tracking systems.

- Source: [Kaggle](https://www.kaggle.com/code/kerneler/starter-change-detection-2014-042f59d1-1/input)
- Format: Pairwise image frames (e.g., t0 and t1)
- Labels: Ground truth masks indicating changed regions

## 🚀 Methodology

The pipeline follows a hybrid approach:

1. **Preprocessing**
   - Grayscale conversion and histogram equalization
   - Image registration if needed

2. **Initial Change Detection**
   - Basic frame differencing
   - Thresholding to identify candidate regions

3. **Rough Entropy Integration**
   - Apply rough set theory to evaluate uncertainty in detected regions
   - Entropy-based refinement to remove noise and improve robustness

4. **Post-Processing**
   - Morphological operations (e.g., dilation, erosion)
   - Tracking visualization using bounding boxes and change masks

5. **Evaluation**
   - Qualitative comparisons
   - Accuracy metrics (IoU, F1-score) on synthetic or labeled ground truths


## 🧠 Current phase

- Research, learning, finding dataset are done.
- First implementation is done, still needs a lot of improvement and testing.