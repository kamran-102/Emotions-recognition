# Emotions Recognition Using CNN

### Overview

This repository contains the code and instructions to train a CNN model for emotion detection in images. The model distinguishes between two classes: "Happy" and "Sad". The primary goal is to create a robust classifier that can accurately predict these emotions based on the facial expressions captured in the images.

### Features

- **Dataset Organization:** Images are stored in a `data/` directory, with subdirectories `happy/` and `sad/` for respective emotions.
- **Data Cleaning:** Automatically checks and removes unsupported image formats (`jpeg`, `jpg`, `bmp`, `png`) to ensure dataset validity.
- **CNN Layers:** Convolutional layers extract key features such as edges and textures, while MaxPooling layers downsample feature maps to reduce dimensionality and     highlight prominent features. Flatten layers convert feature maps into vectors, followed by Dense layers that perform the final classification.
- **Model Training and Evaluation:** The model is trained using the Adam optimizer and categorical cross-entropy loss with training and validation data. Post-training, the model’s accuracy is evaluated on the validation set, and training/validation performance is plotted over epochs.
- **Model Prediction:** The trained model would predict emotions (happy or sad) on new, random images by analyzing the input and provide the corresponding classification.

### Dependencies

- **Python 3.x**
- **TensorFlow**
- **OpenCv**
- **Numpy**
- **Matplotlib**

### Installation

1. **Install Python 3.x:** Ensure that Python 3.x is installed on your system.
2. **Install Required Libraries:** Run the following command to install the necessary Python libraries:
    ```bash
    pip install tensorflow opencv-python numpy matplotlib
    ```
3. **Clone the Repository:** Download or clone this repository to your local machine.


### Notes

- Ensure that your dataset is properly organized and cleaned before starting the training process. Incorrectly labeled or corrupted images can negatively impact model performance.
- It's recommended to run the training on a machine with a GPU for faster computation.
- Hyperparameters like the number of layers, batch size, and learning rate can be fine-tuned for better accuracy depending on the dataset size and complexity.


### Disclaimer

This script is provided for educational purposes only, and the author assumes no liability for any misuse.
