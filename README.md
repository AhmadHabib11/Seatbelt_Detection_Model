# Seatbelt_Detection_Model

Seatbelt Detection using Logistic Regression (From Scratch)
This project implements a binary image classifier to detect whether a driver is wearing a seatbelt or not, using Logistic Regression built entirely from scratch with NumPy — no high-level ML frameworks like sklearn or tensorflow were used.

Overview
Goal: Classify images as “Seatbelt” (safe) or “No Seatbelt” (unsafe).

Approach:

Implemented Logistic Regression from scratch:

Forward & backward propagation

Cost function computation

Gradient descent optimization (vectorized)

Preprocessing: Resizing, normalization, flattening images

Analyzed multiple learning rates using cost graphs to choose optimal

Dataset
Custom dataset (~1000 images) with two classes:

0 → Seatbelt present (safe)

1 → No seatbelt (unsafe)



Preprocessing steps are documented in the notebook.

Results
Trained for 2000 iterations with learning rate = 0.01

Training Accuracy: ~93%

Test Accuracy: ~85%

(Accuracy limited due to logistic regression’s inability to capture spatial features in images.)

Key Learnings
Binary classification with Logistic Regression

Cost function and loss derivation for multiple examples (
1
/
𝑚
1/m factor)

Gradient descent optimization and vectorization

Effect of learning rates on convergence (analyzed via cost plots)

Threshold-based predictions (0.5 cutoff)

Limitations
Logistic Regression struggles with complex visual features (spatial patterns).

Custom dataset size is small; performance drops on unseen internet images.

Predictions sensitive to lighting/angle due to simple preprocessing.

Future Work
Re-implement using Convolutional Neural Networks (CNNs) for better spatial feature extraction.

Expand dataset for more robust real-world performance.

Experiment with data augmentation (brightness, rotation) to improve generalization.
