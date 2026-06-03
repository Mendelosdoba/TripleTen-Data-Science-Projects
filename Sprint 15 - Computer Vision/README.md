
Alcohol Age Classification Using Computer Vision
Project Overview

This project explores whether computer vision can be used to estimate a person's age from facial images and whether such a model could support age verification for alcohol purchases.

A deep learning model based on a pretrained ResNet50 convolutional neural network was trained on facial images to predict a person's age. The primary evaluation metric was Mean Absolute Error (MAE), which measures the average difference between predicted and actual ages.

Business Problem

Retailers must verify that customers are above the legal drinking age before purchasing alcohol. Automated age estimation systems could potentially assist employees by flagging customers who may require ID verification.

The objective of this project was to determine whether a computer vision model can estimate age accurately enough to support this process.

Dataset

The dataset contains:

7,591 facial images
Ages ranging from 1 to 100 years old
Image labels stored in a CSV file
Approximately 29% of individuals aged 21 or younger
Key Statistics
Mean age: ~31 years
Median age: 29 years
Age range: 1–100 years
Standard deviation: ~17 years
Exploratory Data Analysis (EDA)

The age distribution showed:

Strong representation of young and middle-aged adults
Fewer samples among elderly individuals
Slight right skew toward older ages
No significant missing values

The dataset provided a broad range of ages suitable for age prediction tasks.

Data Preparation

Images were processed using TensorFlow's ImageDataGenerator:

Pixel values rescaled from 0–255 to 0–1
Images resized to 224×224 pixels
75% training split
25% validation split
Model Architecture
ResNet50 Transfer Learning

The model uses a pretrained ResNet50 backbone trained on ImageNet.

Architecture:

ResNet50 (pretrained on ImageNet)
GlobalAveragePooling2D
Dense output layer with linear activation
Training Configuration
Framework: TensorFlow / Keras
Optimizer: Adam
Learning Rate: 0.0005
Loss Function: Mean Squared Error (MSE)
Evaluation Metric: Mean Absolute Error (MAE)
Epochs: 20
Results
Final Performance
Validation MAE: approximately 6.7 years

This means that predictions were off by roughly 6–7 years on average.

Business Interpretation

The model successfully learned age-related facial features and produced reasonable age estimates.

However, for legal age verification, an average error of 6–7 years is too large.

Examples of potential risks:

A 17-year-old could be predicted as 23 years old.
A 25-year-old could be predicted as 19 years old.

Because of these errors, the model is not reliable enough to make legal purchasing decisions without human verification.

Conclusion

This project demonstrates that deep learning and transfer learning can effectively estimate age from facial images. The ResNet50 model achieved an MAE of approximately 6–7 years, showing strong predictive capability for general age estimation.

While suitable for demographic analysis, marketing insights, or approximate age estimation, the model is not accurate enough to serve as a standalone alcohol age verification system. It should only be used as a supplementary tool alongside traditional ID verification methods.

Technologies Used
Python
TensorFlow
Keras
ResNet50
NumPy
Pandas
Matplotlib
ImageDataGenerator
