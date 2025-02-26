# Facial Expression Detection Using Key Facial Points

## Overview
This project utilizes key facial points to detect facial expressions. The dataset contains X and Y coordinates of facial landmarks along with corresponding grayscale facial images. The goal is to preprocess, augment, and train a deep learning model for accurate facial expression recognition.

## Features
- Loads and processes a dataset containing facial landmarks and images.
- Converts images from string format to NumPy arrays.
- Performs data augmentation techniques such as:
  - Horizontal flipping
  - Brightness adjustment
  - Vertical flipping
- Normalizes image pixel values for improved model performance.
- Splits data into training and testing sets.
- Implements a deep learning model based on ResNet for facial key point detection.

## Requirements
Install the necessary dependencies using:

```bash
pip install numpy pandas matplotlib seaborn opencv-python tensorflow
```

## File Structure
- `data.csv` - CSV file containing facial landmark coordinates and image pixel values.
- `facial_expression_detection.ipynb` - Jupyter Notebook for data preprocessing, augmentation, and model training.

## How to Run
1. Ensure `data.csv` is available in the working directory.
2. Open `facial_expression_detection.ipynb` in Jupyter Notebook.
3. Run the notebook cells sequentially to preprocess data, augment images, and train the deep learning model.

## Explanation of Key Steps
### Data Preprocessing
- Reads and cleans the dataset.
- Converts image data into NumPy arrays and reshapes them.
- Displays sample images with key facial landmarks.

### Data Augmentation
- Flips images horizontally and adjusts landmark positions accordingly.
- Increases brightness randomly to enhance model robustness.
- Flips images vertically to simulate different viewing angles.
- Combines original and augmented data for a more diverse dataset.

### Normalization
- Scales pixel values to the range [0,1] to improve neural network training.

### Model Training
- Splits data into training and testing sets.
- Implements a ResNet-based deep learning model for feature extraction.
- Uses Adam optimizer and loss functions suitable for key point regression.
- Evaluates model performance on test data.

## Output
- Trained model capable of detecting facial key points.
- Visualizations of detected key points on facial images.
- Augmented dataset with improved variation.

## License
This project is open-source and can be used for educational and research purposes.

