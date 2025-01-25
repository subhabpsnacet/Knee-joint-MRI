Dataset Guidelines
Dataset Access:
"The dataset can be accessed at [link].

Data Structure:
"Each image is labeled with its corresponding OA grade (e.g., Grade 0, 1, 2, 3, or 4). Images are stored in .jpg format with the associated labels provided in a labels.csv file."

Preprocessing Guidelines
Preprocessing Steps:
"Before feeding the images into the model, they were resized to 256x256 pixels, normalized to have values between 0 and 1, and augmented with rotations and flips to improve generalization."
Model Training Guidelines
Model Training Settings:
"The GAO-Bi-LSTM was trained with the following parameters:
Learning Rate: 0.001
Batch Size: 32
Epochs: 50
Optimizer: Gaussian Aquila Optimizer (GAO)
A 70:30 train-test split was used, and validation accuracy was monitored for early stopping."
Metrics Calculation Guidelines
Evaluation Metrics:
"The following metrics were calculated:

Sensitivity and Specificity: True positive and true negative rates using a 0.5 threshold.
Accuracy: Ratio of correctly predicted samples to total samples.
Segmentation Dice Coefficient: Overlap measure between predicted and ground truth segmentations.
