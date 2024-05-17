# Table of content  
### 1. Introduction    
* Overview of using CNNs to diagnose pneumonia from chest X-ray images.                       
* Explanation of the project's aim to enhance diagnostic accuracy using advanced technology.   

### 2. Dataset Overview  
Description of the "Chest X-Ray Images (Pneumonia)" dataset sourced from Kaggle.  <br>
Organization of data into train, test, and validation sets with categories for Pneumonia and Normal images. 

### 3. Models Employed
Details on the conventional CNN model built for direct image learning. <br>
Overview of the pretrained VGG16 model and its fine-tuning for enhanced feature extraction.

### 4. Model Structures and Functionalities
#### Conventional CNN Model:
* Architecture from input to output layers.
* Explanation of each layer's function including convolutional, max pooling, dense, and dropout layers.

#### VGG16 Model:
*Composition of the VGG16 network.
* Adjustments made for pneumonia classification and the rationale behind using pretrained models.

### 5. Model Evaluation and Implementation
####  Data Preprocessing:
- Techniques for loading, resizing, and augmenting the data.
- Importance of normalization.

#### Model Training and Compilation:
- Configuration of models including optimizer and loss function selection.
- Training duration and conditions.

####  Model Validation and Testing:
- Split details and methodology for training/validation/testing.
- Use of ROC curve and AUC for performance evaluation.  <br>

### 6. Results and Discussion
* Presentation of training outcomes, accuracy, and loss metrics.
* Discussion on overfitting observed during validation and the steps taken to address it.

### 7. Conclusion
* Summary of the study's findings.
* Assessment of the models' effectiveness in improving pneumonia diagnostics.
* Future directions for research to enhance model generalizability.

### 8. References
* Comprehensive listing of all sources cited in the report.












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







