# Grass-Weed-Detection-Model


1. *train.py* : Training the Model
  Objective: Train a classification model using TensorFlow and Keras, leveraging the InceptionV3 architecture with custom classification layers.
Key Features:
  Data Augmentation: Aggressive transformations for training and moderate ones for validation using ImageDataGenerator.
  Model Architecture: Uses a pretrained InceptionV3 model with added layers for task-specific classification.
  Optimization: Implements Adam optimizer with a custom learning rate schedule.
  Callbacks: Includes EarlyStopping, ModelCheckpoint, and ReduceLROnPlateau for enhanced training control.
Output: Saves the trained model in .keras format.


2. *predict.py* : Prediction and Visualization
  Objective: Predict the class of a new image and visualize activation maps.
Key Features:
  Prediction: Accepts an image path, preprocesses the image, and predicts using the saved model.
  Grad-CAM Heatmap: Generates a heatmap to interpret the model's focus areas on the image, using gradient-based techniques.
  Visualization: Creates superimposed images for better insights.


3. *app.py* : Web Application
  Objective: Provide a user-friendly interface for image uploads, predictions, and visualizations.
Key Features:
  Flask Web Interface: Handles file uploads and serves predictions with Grad-CAM overlays.
  Image Storage: Saves uploaded images and generated heatmaps to a static folder for display.
  Dynamic Rendering: Displays results including predictions and visualizations on the web page.
  Routing: Manages home (/) and file retrieval routes for seamless interaction.





