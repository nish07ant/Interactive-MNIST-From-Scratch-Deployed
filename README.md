# Interactive MNIST Digit Recognition From Scratch

This project implements a neural network from scratch to recognize handwritten digits using the MNIST dataset. It includes an interactive drawing canvas where you can draw your own digits and test the model's predictions.

## Overview

The MNIST dataset is a collection of 70,000 handwritten digits (60,000 for training and 10,000 for testing), each represented as a 28x28 pixel grayscale image. This project:

1. Loads and processes the MNIST dataset
2. Builds a neural network from scratch using NumPy
3. Trains the model on the MNIST dataset
4. Provides an interactive canvas to draw digits and test the model

## Features

- **Neural Network Implementation**: A fully-connected neural network with 3 layers built from scratch using only NumPy
- **Data Processing**: Conversion of MNIST ubyte format to CSV
- **Interactive Testing**: Draw your own digits using a Tkinter-based canvas and test the model's predictions
- **Visualization**: Display of training progress and prediction results

## Requirements

- Python 3.6+
- NumPy
- Pandas
- Matplotlib
- Pillow (PIL)
- Tkinter (usually comes with Python)

## Installation

1. Clone this repository:
   ```
   git clone https://github.com/yourusername/Interactive-MNIST-From-Scratch.git
   cd Interactive-MNIST-From-Scratch
   ```

2. Install the required packages:
   ```
   pip install -r requirements.txt
   ```

3. Run the Jupyter notebook:
   ```
   jupyter notebook digit_classifier.ipynb
   ```

## Dataset

The MNIST dataset is included in the `data` directory in its original ubyte format:
- `train-images.idx3-ubyte`: Training images (60,000)
- `train-labels.idx1-ubyte`: Training labels
- `t10k-images.idx3-ubyte`: Test images (10,000)
- `t10k-labels.idx1-ubyte`: Test labels

The notebook converts these files to CSV format for easier processing.

## Neural Network Architecture

The neural network has the following architecture:
- Input layer: 784 neurons (28x28 pixels)
- Hidden layer 1: 128 neurons with ReLU activation
- Hidden layer 2: 64 neurons with ReLU activation
- Output layer: 10 neurons with Softmax activation

The model is trained using mini-batch gradient descent with a learning rate of 0.1 for 100 epochs.

## Usage

1. Open the `digit_classifier.ipynb` notebook
2. Run all cells to train the model
3. Use the interactive canvas to draw your own digits
4. The model will predict the digit you've drawn

## Interactive Drawing

The project includes a Tkinter-based drawing canvas where you can:
1. Draw a digit using your mouse
2. Clear the canvas if needed
3. Submit your drawing for prediction
4. See the model's prediction

## License

[MIT License](LICENSE)

## Acknowledgments

- The MNIST dataset was created by Yann LeCun, Corinna Cortes, and Christopher J.C. Burges
- This project was inspired by the desire to understand neural networks at a fundamental level
