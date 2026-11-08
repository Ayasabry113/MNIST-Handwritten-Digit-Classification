# MNIST Handwritten Digit Classification

A machine learning and deep learning comparison project for classifying handwritten digits (0–9) using the MNIST dataset.

## Models
- Artificial Neural Network (ANN): compares different hidden-layer sizes.
- Support Vector Machine (SVM): compares linear, RBF, and polynomial kernels.
- Convolutional Neural Network (CNN): trains a CNN with validation-based early stopping.

## Dataset
The notebook loads MNIST automatically using `tensorflow.keras.datasets`. **You do not need to download or upload a dataset folder manually.** The first run may require an internet connection so Keras can download MNIST.

## Project files
- `MNIST_Handwritten_Digit_Classification.ipynb` — complete, documented notebook.
- `requirements.txt` — Python dependencies.

## Run locally
```bash
python -m venv .venv
# Windows:
.venv\Scripts\activate
# macOS/Linux:
source .venv/bin/activate

pip install -r requirements.txt
jupyter notebook
```
Open `MNIST_Handwritten_Digit_Classification.ipynb` and run the cells from top to bottom.

## Notes
- SVM experiments use a stratified 10,000-image subset to keep training time manageable.
- ANN comparison uses a validation split from the training data.
- CNN uses a validation split for early stopping and evaluates the official test set after training.
- Training time and accuracy can vary depending on hardware and software versions.

## Technologies
Python, TensorFlow/Keras, NumPy, Pandas, Matplotlib, Seaborn, and Scikit-learn.
