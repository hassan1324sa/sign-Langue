# Gesture Recognition Using CNN

This project implements a convolutional neural network (CNN) for gesture recognition using images. The model is trained to classify gestures based on images stored in separate folders for each gesture category.

## Table of Contents
- [Introduction](#introduction)
- [Installation](#installation)
- [Dataset](#dataset)
- [Usage](#usage)
- [Model Architecture](#model-architecture)
- [Training](#training)
- [Evaluation](#evaluation)
- [Results](#results)
- [License](#license)

## Introduction

The goal of this project is to recognize hand gestures using a deep learning model. This can be applied in various fields such as human-computer interaction, gaming, and sign language recognition. The model is built using TensorFlow and Keras.

## Installation

To run this project, you need to have Python installed along with the following libraries:

```bash
pip install opencv-python mediapipe numpy tensorflow matplotlib scikit-learn
```
# Dataset

The dataset is organized into separate folders for each gesture category under the train directory. The following categories are included:

- Bye
- Hello
- Hey
- Lol
- Welcome
- Thanks
Each category folder should contain images of the corresponding gestures.

# Usage
1. Clone the repository:
   ```bash
      git clone https://github.com/yourusername/gesture-recognition.git
      cd gesture-recognition
   ```
2. Prepare your dataset by organizing images into the train directory as described above.
3. Run the script to train the model:
  ```bash
  python your_script_name.py
  ```
4. After training, you can test the model with a sample image. Ensure that the test image is available in the test directory.

# Model Architecture
The model architecture consists of:
  - Convolutional layers for feature extraction
  - Max pooling layers for downsampling
  - Flattening layer to convert 2D features into 1D
  - Fully connected layers for classification
  - Dropout layer for regularization
  The model is compiled using the Adam optimizer and sparse categorical crossentropy as the loss function.
 
# Training
The model is trained for 20 epochs with a batch size of 32. The training process includes data augmentation and normalization to improve model performance.


# Evaluation
After training, the model's performance can be evaluated on a test set. The evaluation metrics include accuracy and loss.

# Results
The model predicts the class of the test images. Predictions can be visualized to assess the model's performance.

# License
This project is licensed under the MIT License. See the LICENSE file for more information.

### Notes for Customization
- **Repository URL**: Replace `https://github.com/yourusername/gesture-recognition.git` with the actual URL of your GitHub repository.
- **Script Name**: Replace `your_script_name.py` with the actual name of your Python script that contains the CNN implementation.
- **Dataset Description**: Add any additional details about the dataset if necessary, such as image resolution or size.
- **License**: Adjust the license section according to the license you choose for your project.

Feel free to modify any sections to better fit your project's details or your personal preferences!


