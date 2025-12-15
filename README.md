# DanseNet_snake_project

 ###File Overview
 - Predicts the species of a snake from a single image using the trained model. Shows the image with species name, biological name, venom status, and similar species.
 - Reads the snake_data.csv file and prints the number of rows. Useful to verify your dataset.
 - Defines a custom PyTorch Dataset class (SnakeDataset) to load images and labels from CSV for training or inference.
 - Simple GUI for selecting an image file using Tkinter. Currently prints the selected file path.
 - Loads a pretrained DenseNet121 model and replaces the classifier layer with one matching the number of species in your dataset.
 - GUI wrapper to run predict_image() on a selected image. Combines select_image.py and predict.py functionality.
 - Trains the DenseNet model using SnakeDataset. Uses augmentation, normalization, DataLoader batching, and saves the trained model to model.pth.
 - Visualizes predictions on the entire dataset. Shows images with predicted vs. true species labels.

  ###Features
  - Train a DenseNet121 model to classify snake species.
  - Load and preprocess images with PyTorch Dataset.
  - Predict species for a single image with GUI selection.
  - View predictions along with biological name, venom status, and similar species.
  - Visualize predictions vs ground truth for the whole dataset.
  - Works with GPU if available.

  ###Tech
  - Python

  ###Installation
  - Clone the repository [git clone https://github.com/Yamipyae/DanseNet_snake_project.git  # Replace with your repo
  - cd <repo_name>
  - pip install torch torchvision pandas pillow matplotlib
  - Prepare files
    - Place snake_data.csv in data/.
    - Place snake images in data/images/.
  - Train the model
    - python train.py
    - Saves model as model.pth.
  - Run predictions
    - python run_predict.py
  - Visualize predictions
    - python visualize.py

  ###Example Output
  - Predicted Species: Cobra
  - Biological Name: Naja naja
  - Venom: Highly venomous
  - Similar Species: King Cobra


