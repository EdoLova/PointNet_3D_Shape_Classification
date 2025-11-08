# PointNet 3D Shape Classification

This project implements a **PointNet** model for 3D shape classification from point clouds. It includes a full PyTorch pipeline for training, evaluation, and robustness testing against noise. Data augmentation is applied to improve generalization.

## Objectives
- Classify 3D geometric shapes (cylinders, rectangular parallelepipeds, tori) from point clouds.
- Train and evaluate a PointNet model using PyTorch.
- Compute classification metrics: accuracy, precision, recall, F1-score.
- Test model robustness with noisy data.
- Apply data augmentation to improve generalization.

## Tools and Libraries
- **Python**, PyTorch, Numpy, Matplotlib, scikit-learn
- Dataset: synthetic 3D point clouds generated with `prepare_data.py`

## Setup
1. Clone this repository.
2. Install dependencies:
   pip install numpy matplotlib torch scikit-learn

## How to Run
1. Generate the dataset:
   python prepare_data.py
2. Train the PointNet model and evaluate:
   python tp_soluzione_gcolab.py
   - This will train the model and save it as `mypointnet.pt`.
   - Confusion matrices and metrics (accuracy, precision, recall, F1-score) will be displayed.
   - Noise robustness and data augmentation tests are included in the script.
   
## Main Results
- High classification accuracy for all 3 classes.
- Confusion matrices show clear separation between shape types.
- Model remains robust under Gaussian noise with σ up to 0.02.
- Data augmentation further improves generalization on noisy inputs.

## Author
Edoardo Lovato  
Université Claude Bernard Lyon 1 
Master DISS - Fundamentals Of Image Processing And Interpretation 
Academic Year 2025–2026
