# Handwritten Alphabet Recognition

This project implements a deep learning model using TensorFlow and Keras to 
accurately recognize handwritten alphabet characters from images. 
The trained model can predict letters from user-supplied images.

## Contents

- **`Handwritten-Alphabets-Recognition.ipynb`**: Jupyter Notebook for training the model, visualizing its performance, and saving it.
- **`Test_Handwritten-Alphabets-Model.ipynb`**: Python script to load the saved model and make predictions on new images.
- **`test_model`**: Directory to store user-provided images for prediction.
- **`handwritten_alphabets.keras`**: Saved model file containing the trained neural network weights and architecture.

## Training the Model

The model architecture consists of:
- **Input Layer**: Flatten layer that converts 28x28 pixel images into a 784-dimensional vector.
- **First Hidden Layer**: Dense layer with 1024 units and ReLU activation.
- **Second Hidden Layer**: Dense layer with 512 units and ReLU activation.
- **Third Hidden Layer**: Dense layer with 128 units and ReLU activation.
- **Output Layer**: Dense layer with 26 units and softmax activation for multi-class classification (one unit per letter A-Z).

Open `Handwritten-Alphabets-Recognition.ipynb` in Jupyter Notebook and run all cells to train the model if u want makechange it, evaluate its performance, and save it as `handwritten_alphabets.keras`.

## Making Predictions

To make predictions on new images:
1. Place your images in the `test_model/` folder. Ensure that the images are in PNG format and named appropriately.
2. Run the `Test_Handwritten-Alphabets-Model.ipynb` script. This script will:
   - Load the saved model from `handwritten_alphabets.keras`.
   - Process the images in the `test_model/` folder.
   - Display the predictions along with the input images.