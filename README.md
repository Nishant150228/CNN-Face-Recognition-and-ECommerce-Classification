# Facial Recognition and E-commerce Analysis Projects  

## Task 1: Facial Recognition with CNN  

### Introduction  
Convolutional Neural Networks (CNNs) are highly effective for facial recognition due to their ability to automatically learn features from images, such as edges, textures, and complex patterns. This makes CNNs ideal for distinguishing subtle facial details like expressions and lighting variations, leading to high accuracy in identifying individuals. Applications include security, surveillance, and personalized user experiences.  

### Dataset Description  

#### ORL Database of Faces (AT&T Database of Faces)  
The ORL Database of Faces is a widely used dataset for facial recognition and image classification tasks.  

**Key Features:**  
- **Total Images**: 400 grayscale images.  
- **Subjects**: 40 individuals with 10 images each.  
- **Variations**:  
  - Lighting conditions.  
  - Expressions: Open/closed eyes, smiling/not smiling.  
  - Facial details: With/without glasses.  
  - Head positions: Upright with minor side movements.  
- **Image Specs**:  
  - Size: 92x112 pixels.  
  - Gray Levels: 256 levels per pixel.  
- **Background**: Homogeneous, dark background with upright, frontal poses.  

**Dataset Link**: [Download from Kaggle](https://www.kaggle.com/datasets/kasikrit/att-database-of-faces).  

### Model Overview  

- **Total Parameters**: 52,500,114 (200.27 MB)  
- **Trainable Parameters**: 52,500,114  
- **Non-Trainable Parameters**: 0  

#### Layer-by-Layer Breakdown  

1. **Conv2D Layers**: Extract features with filters and kernel sizes.  
2. **MaxPooling Layers**: Reduce dimensionality and focus on key features.  
3. **Flatten Layer**: Converts outputs to a 1D vector.  
4. **Dense Layers**: Perform high-level learning for classification.  
5. **Dropout Layers**: Prevent overfitting.  

**Summary**: The architecture combines convolutional and dense layers for feature extraction and classification.  

### Model Performance  

- **Test Accuracy**: 93.75%  
- **Test Loss**: 0.4115  

**Interpretation**: High accuracy and low loss indicate effective learning and generalization on unseen data.  

---  

## Task 2: E-commerce Analysis  

### Dataset Description  

The E-commerce Sales Data dataset provides insights into user profiles, product details, and user-product interactions.  

#### Dataset Structure  

- **User Sheet**: User profiles with attributes like ID, name, age, and location.  
- **Product Sheet**: Details of products, including IDs, categories, and prices.  
- **Interactions Sheet**: Logs of user actions like views, purchases, reviews, and ratings.  

### Model Performance Metrics  

#### Mean Squared Error (MSE):  

- **Training MSE**: 0.0192  
- **Validation MSE**: 0.0454  
- **Test MSE**: 0.0436  

#### R-squared:  

- **Training**: 0.5028  
- **Validation**: -0.2223  
- **Test**: -0.1555  

### Interpretation  

The model performs well on training data but struggles on validation and test sets, as indicated by negative R-squared values. Improvements could involve hyperparameter tuning, model adjustments, or additional data collection.  

---  
