This GitHub repository contains a machine learning project focused on diagnosing pneumonia from chest X-ray images using Convolutional Neural Networks (CNNs). The project employs two different models: a conventional CNN built from scratch and a pre-trained VGG16 model, optimized for image classification.

The project utilized two models for the classification of pneumonia from chest X-ray images, each demonstrating distinct characteristics and strengths in handling medical imaging data.

Conventional CNN Model
The conventional CNN model is custom-designed specifically for this task. It consists of a series of convolutional layers that progressively extract features from the images, followed by max pooling layers that reduce the dimensionality of the data, thereby simplifying the image inputs without losing critical information. The network also includes dense layers with a high number of neurons to facilitate complex pattern recognition and a dropout layer to prevent overfitting by randomly ignoring some neurons during training. This model is structured to learn directly from the raw images and adaptively improve its parameters through backpropagation. Trained over 50 epochs, it reached a high training accuracy of approximately 94.70%, although it exhibited some fluctuations in validation loss, indicating potential overfitting issues.

VGG16 Model
The VGG16 model leverages the architecture from an existing deep network pre-trained on the ImageNet dataset. This model is known for its deep architecture consisting of 16 layers and its ability to perform well on a wide range of image recognition tasks due to its comprehensive and robust training on a diverse set of images from ImageNet. For this project, the VGG16 was adapted for binary classification by modifying the top layers to suit the pneumonia vs. normal classification task and freezing the initial layers to retain the learned features. The transfer learning approach allows the VGG16 model to utilize learned features, significantly reducing the need for extensive data specific to the task at hand. It showed a slightly lower accuracy of about 92.8% but demonstrated better generalization on validation data, evidenced by more stable loss metrics across epochs.

Citation: http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5





