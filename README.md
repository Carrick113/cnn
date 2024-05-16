This GitHub repository contains a machine learning project focused on diagnosing pneumonia from chest X-ray images using Convolutional Neural Networks (CNNs). The project employs two different models: a conventional CNN built from scratch and a pre-trained VGG16 model, optimized for image classification.

The project utilized two models for the classification of pneumonia from chest X-ray images, each demonstrating distinct characteristics and strengths in handling medical imaging data.

Conventional CNN Model
The conventional CNN model is custom-designed specifically for this task. It consists of a series of convolutional layers that progressively extract features from the images, followed by max pooling layers that reduce the dimensionality of the data, thereby simplifying the image inputs without losing critical information. The network also includes dense layers with a high number of neurons to facilitate complex pattern recognition and a dropout layer to prevent overfitting by randomly ignoring some neurons during training. This model is structured to learn directly from the raw images and adaptively improve its parameters through backpropagation. Trained over 50 epochs, it reached a high training accuracy of approximately 94.70%, although it exhibited some fluctuations in validation loss, indicating potential overfitting issues.

VGG16 Model
The VGG16 model leverages the architecture from an existing deep network pre-trained on the ImageNet dataset. This model is known for its deep architecture consisting of 16 layers and its ability to perform well on a wide range of image recognition tasks due to its comprehensive and robust training on a diverse set of images from ImageNet. For this project, the VGG16 was adapted for binary classification by modifying the top layers to suit the pneumonia vs. normal classification task and freezing the initial layers to retain the learned features. The transfer learning approach allows the VGG16 model to utilize learned features, significantly reducing the need for extensive data specific to the task at hand. It showed a slightly lower accuracy of about 92.8% but demonstrated better generalization on validation data, evidenced by more stable loss metrics across epochs.

Both models showcase the potential of CNNs in medical diagnostics, with the conventional CNN excelling in sensitivity and the VGG16 in specificity, making them valuable tools for enhancing clinical diagnostic processes.

Preprocessing scripts for image cleaning, augmentation, normalization, and resizing to prepare the data for training.
Training scripts showcasing the configuration and execution of both CNN models.
Evaluation scripts used to assess model performance through accuracy, loss metrics, confusion matrices, ROC curves, and AUC scores.
A comprehensive set of results that detail the models' performance over various training epochs, highlighting their effectiveness in clinical diagnostics.
This project aims to demonstrate the potential of AI in medical imaging, providing a robust framework for detecting pneumonia, which can be extended or adapted for other image classification tasks in healthcare.

Repository Structure
/data_preprocessing/: Contains scripts for data cleaning, augmentation, normalization, and resizing. This ensures the X-ray images are optimally prepared for model training.
/models/: Includes Python scripts for building and training the conventional CNN and VGG16 models. Model configurations, hyperparameters, and training procedures are detailed within these scripts.
/evaluation/: Scripts for evaluating the models using various metrics such as accuracy, precision, recall, F1 score, and ROC curves. Includes functions to plot confusion matrices and calculate loss statistics.
/results/: Stores output files like model weights, training logs, and visualizations of performance metrics across training and validation phases.
/docs/: Documentation files explaining the project's methodology, setup, and usage instructions.
