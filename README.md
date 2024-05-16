# Table of content

### 1. Introduction
This project utilizes Convolutional Neural Networks (CNNs) to diagnose pneumonia from chest X-ray images, aiming to enhance the accuracy and efficiency of medical diagnostics. The study's significance lies in its potential to improve patient outcomes through quicker, more accurate diagnoses. The project utilizes two CNN models:  <br>
- a custom-designed conventional CNN for direct learning from X-rays, <br>
- and a pretrained VGG16 model, fine-tuned for enhanced feature extraction.
<br>
<br>


### 2. Data Collection
- Source of Data, http://www.cell.com/cell/fulltext/S0092-8674(18)30154-5 <br>
* Dataset Description <br>
![jZqpV51](https://github.com/Carrick113/cnn/assets/138642124/ec5ab25b-a2af-4e78-98ad-b8f9d1339c2d) <br>
The dataset is organized into 3 folders (train, test, val) and contains subfolders for each image category (Pneumonia/Normal). There are 5,863 X-Ray images (JPEG) and 2 categories (Pneumonia/Normal).


### 3. Data Cleaning <br>
#### Data Augmentation/ Data Normalization/ Image Resizing <br>
Data augmentation (Figure 1) through rotation, zoom, and flipping increased variability, improving model robustness. Data normalization (Figure 2) scaled pixel values between 0 and 1, enhancing training stability. Resizing images to 224x224 pixels (Figure 3) ensured consistent input dimensions for the models.<br>

### 4. Model Development
Conventional CNN Model <br>
After 50 epochs, it shows improvement but struggles with high validation losses, suggesting overfitting. Fluctuating validation accuracy and soaring loss indicate issues in generalizing to new data, highlighting need for better regularization. <br>
![image](https://github.com/Carrick113/cnn/assets/138642124/329d52c2-694f-4569-94f9-0387122aa3bb) <br>
Evaluate model and display result <br>
![image](https://github.com/Carrick113/cnn/assets/138642124/b2b865da-d1d4-4a46-a85f-aaf0bd63919b)   <br>





VGG16 Model
Architecture Description
Adaptation for Pneumonia Detection
Training Process

### 5. Model Evaluation
Evaluation Metrics
Accuracy and Loss Analysis
Confusion Matrices
ROC Curves and AUC Scores

### 6. Results
Performance Comparison
Model Selection
Discussion on Overfitting and Generalization

### 7. Discussion
Insights and Findings
Comparison with Existing Methods

### 8. Conclusions
Summary of Findings
Implications for Clinical Practice

### 9.Future Work
Recommendations for Further Research
Potential Improvements in Model Architecture

### 10. References




