# ANN-DigitRecognizer
# Deep Learning Image Classification with MNIST Dataset

## Project Overview
The ANN-DigitRecognizer project is designed to classify handwritten digits using an Artificial Neural Network (ANN) architecture. Leveraging the MNIST dataset, this model achieves high accuracy in recognizing and predicting digit images. This project demonstrates the power of deep learning techniques in solving real-world classification problems.

## Dataset

The dataset used in this project is the MNIST dataset, which consists of:
- **Training Images**: 60,000 images of handwritten digits.
- **Test Images**: 10,000 images for evaluation.
  
The images are 28x28 pixels in grayscale format.

## Technologies Used
- Python
- TensorFlow/Keras
- NumPy
- Matplotlib
- scikit-learn

## Kaggle Link
You can find the project on Kaggle at the following link: [ANN-DigitRecognizer](https://www.kaggle.com/code/haticebaydemir/ann-digitrecognizer) 


## Model Architecture

The model consists of the following layers:
1. **Input Layer**: Takes flattened input images of shape 784 (28x28 pixels).
2. **Hidden Layers**:
   - First hidden layer with 512 neurons and ReLU activation.
   - Dropout layer to prevent overfitting.
   - Second hidden layer with 256 neurons and ReLU activation.
   - Dropout layer for regularization.
   - Third hidden layer with 128 neurons and ReLU activation.
   - Dropout layer for further regularization.
3. **Output Layer**: Softmax activation for multi-class classification (10 classes for digits 0-9).


## Installation

To get started with this project, clone the repository and install the necessary dependencies:

```bash
git clone https://github.com/yourusername/ANN-DigitRecognizer.git
cd ANN-DigitRecognizer
pip install -r requirements.txt
```

## Usage
To train the model, run the following command:
```bash
python train.py
```
After training, you can evaluate the model with the test dataset by running:
```bash
python evaluate.py
```

## Results
Upon training, the model achieved the following performance metrics on the test dataset:

- **Test Loss**: 0.0721
- **Test Accuracy**: 98.09%
These results demonstrate the model's effectiveness in accurately classifying handwritten digits.

## Contributing
Contributions to improve the project are welcome! Please fork the repository and submit a pull request for any enhancements or fixes.

## Contact
For any questions or suggestions, please feel free to reach out using the contact information below:

Email: baydemirhatice@hotmail.com

LinkedIn: Hatice Baydemir
