# Building and Evaluating Neural Networks for MNIST

## Overview 
This project focuses on building, training, and evaluating several neural network architectures on the MNIST dataset of handwritten digits using PyTorch.
The goal is to compare the performance of different architectures, from a simple single hidden layer to a convolutional neural network (CNN), and analyze their accuracy and learning behavior.

## Project Structure 
```text
deep_learning/
├── data/                    # MNIST dataset (downloaded automatically)
├── code_for_project.ipynb   # Main Jupyter notebook (training + evaluation)
├── report_of_project.pdf    # Full report with methods, results, and appendices
└── README.md                # Project documentation
```

## How to run
### Requirements

Make sure you have Python ≥ 3.9.
You can install dependencies using:
```text
pip install torch torchvision matplotlib pandas
```

### Run the notebook
Open the Jupyter notebook and execute all cells:
```text
jupyter notebook code_for_project.ipynb
```

The code will:

1) Download the MNIST dataset automatically.

2) Train and evaluate three neural network models.

3) Print and plot the accuracy after each epoch.


## Technical details 
### Libraries used
- torch, torchvision
- matplotlib
- pandas

### Datasets
- MNIST: 60,000 training and 10,000 test grayscale images (28×28 pixels).

### Architecture implemented

| Model                      | Description                   | Accuracy  |
| -------------------------- | ----------------------------- | --------- |
| **Single hidden-layer NN** | 1 hidden layer (400 neurons)  | ≈ 92.5 %  |
| **Two hidden-layer NN**    | Layers of 500 and 300 neurons | ≈ 97.99 % |
| **Convolutional NN (CNN)** | 2 conv layers + dense layers  | ≈ 99.1 %  |
