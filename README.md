# Parking Occupancy Detection Using Convolutional Neural Networks
**By:** Maria Isabel Arango Palacio, Isabella Montoya Henao, Jose Alejandro Villamizar, and María José Bernal Vélez


## Introduction
On average, people can spend up to seven minutes searching for a parking spot, especially in high-traffic urban areas, an inefficiency that contributes to congestion, stress, and wasted fuel. Traditional solutions to this problem often involve costly sensor-based systems installed in enclosed parking structures, limiting their scalability and practicality in open environments. 

To offer a more accessible and cost-effective alternative, this project proposes the use of convolutional neural networks (CNNs) to detect the occupancy status of individual parking spaces using images captured by cameras.

## Repository Structure
This repository contains the following files:
- **requirements.txt:** Python dependencies required to run the notebook.
- **cnn.py:** Jupyter Notebook implementing the CNN architecture, training loop, evaluation, and visualizations.
- **CNRPark-Patches-150x150:** Contains 150x150 image patches labeled as occupied or empty, used for training and testing the CNN.

## Getting Started
### 1. Clone the repository
```
git clone https://github.com/imontoyah/CNN-parking-detection.git
cd CNN-parking-detection
```

### 2. Install dependencies
It’s recommended to use a virtual environment.
```
pip install -r requirements.txt
```

### 3. Run the Notebook
```
jupyter notebook cnn.ipynb
```
Make sure the `CNRPark-Patches-150x150` folder is in the same directory for the notebook to access image data.
In the notebook you can run cell by cell to visualize every step of the CNN Implementation.

## Model Description
The CNN model takes 150x150 pixel images of individual parking spots and classifies each as occupied or empty. The architecture includes convolutional layers, ReLU activations, pooling, and dense layers, trained on a balanced dataset of labeled image patches.

## Results
Evaluation metrics such as accuracy, confusion matrix, and visual output of predictions are displayed at the end of the notebook.

## Dataset
This project uses the CNRPark + EXT dataset, a benchmark for intelligent parking systems. Only a subset of cropped patches is included in this repository. For the full dataset, visit this [link](http://cnrpark.it).
