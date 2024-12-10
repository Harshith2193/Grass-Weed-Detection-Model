# Grass-Weed-Detection-Model


1. *train.py* : Training the Model
  Objective: Train a classification model using TensorFlow and Keras, leveraging the InceptionV3 architecture with custom classification layers.
Key Features:
  Data Augmentation: Aggressive transformations for training and moderate ones for validation using ImageDataGenerator.
  Model Architecture: Uses a pretrained InceptionV3 model with added layers for task-specific classification.
  Optimization: Implements Adam optimizer with a custom learning rate schedule.
  Callbacks: Includes EarlyStopping, ModelCheckpoint, and ReduceLROnPlateau for enhanced training control.
Output: Saves the trained model in .keras format.


