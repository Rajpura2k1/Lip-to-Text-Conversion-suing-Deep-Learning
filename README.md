# Lip-to-Text-Conversion-using-Deep-Learning


## Overview

This project demonstrates a deep learning model for converting lip movements in video sequences into corresponding text. Leveraging the power of Convolutional Neural Networks (CNNs) and Recurrent Neural Networks (RNNs), specifically Long Short-Term Memory (LSTM) units, this project aims to provide an efficient and accurate system for lip reading.

## Table of Contents

1. [Installation](#installation)
2. [Usage](#usage)
3. [Dataset](#dataset)
4. [Model Architecture](#model-architecture)
5. [Training](#training)
6. [Prediction](#prediction)
7. [Results](#results)
8. [Contributing](#contributing)
9. [License](#license)

## Installation

### Prerequisites

- Python 3.7+
- Pip (Python package installer)

### Required Libraries

The following Python libraries are required for this project:

- OpenCV
- Matplotlib
- Imageio
- Gdown
- TensorFlow

## Usage

### Clone the Repository

Clone the repository and navigate to the project directory:

```bash
git clone https://github.com/Rajpura2k1/Lip-to-Text-Conversion-using-Deep-Learning.git
cd lip-to-text-conversion
```

## Dataset

The dataset used in this project can be downloaded using `gdown` Uncomment and run the corresponding lines in the provided Jupyter notebook to download and extract the dataset.

This project uses a dataset consisting of video sequences and their corresponding text alignments. Each video sequence captures the lip movements of a person speaking a sentence.
- Videos: Located in the `data/s1` directory.
- Alignments: Located in the `data/alignments/s1` directory.

## Model Architecture

The model architecture consists of the following layers:

1. 3D Convolutional Layers: These layers capture spatial and temporal features from the video frames.
2. Max Pooling Layers: These layers are used for down-sampling the feature maps.
3. Bidirectional LSTM Layers: These layers capture the temporal dependencies in the sequences by processing the input data in both forward and backward directions.
4. Dense Layer: This layer outputs the character probabilities, enabling the model to predict the corresponding text for the given video frames.

## Training

The model is trained using a dataset of video sequences and their corresponding text alignments. During training, checkpoints are saved to avoid losing progress, and various callbacks are used to monitor and adjust the learning process.

### Checkpoints

Model checkpoints are saved during training to allow resuming from the last saved state. Pre-trained checkpoints can also be downloaded for evaluation or further training.

## Prediction

The trained model can be used to make predictions on new video sequences. The model processes the input video frames and outputs the predicted text alignments.

## Results

The performance of the model can be evaluated by computing the accuracy of the predicted text alignments against the ground truth alignments. This helps in assessing the effectiveness of the model in converting lip movements to text.




