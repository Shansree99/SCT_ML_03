# SCT_ML_03


hello friends this is 
# Cats vs Dogs Classification using SVM

A simple implementation of Support Vector Machine (SVM) to classify images of cats and dogs.

# Overview

This project demonstrates how to:
- Automatically download and preprocess the Oxford-IIIT Pets dataset
- Extract features and prepare data for machine learning
- Train an SVM classifier for binary image classification
- Evaluate model performance and visualize predictions

# Requirements

- Python 3.6+
- Required packages:
  ```bash
  pip install torch torchvision scikit-learn matplotlib numpy
  ```

# Dataset

The code automatically downloads the [Oxford-IIIT Pets Dataset](https://www.robots.ox.ac.uk/~vgg/data/pets/) which contains:
- 37 categories of pets
- ~200 images for each class
- 25% cat images (classes 0-18)
- 75% dog images (classes 19-37)

#How to Run

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/cats-vs-dogs-svm.git
   cd cats-vs-dogs-svm
   ```

2. Run the classification script:
   ```bash
   python cats_vs_dogs_svm.py
   ```

3. The script will:
   - Download the dataset (about 800MB)
   - Preprocess images (resize to 64x64, convert to grayscale)
   - Train an SVM classifier
   - Display accuracy and sample predictions

# Expected Output

After running, you should see:
```
Downloading dataset...
Processing images...
Training SVM...
Accuracy: 0.72

Displaying sample predictions...
```
![Sample predictions](sample_predictions.png)

# Customization

You can modify these parameters in the code:
- Image size (currently 64x64)
- Number of training samples (currently 1000)
- SVM kernel (currently 'linear')
- Color vs grayscale images

# Performance

With default settings:
- Training time: ~1-2 minutes on CPU
- Accuracy: ~70-75%
- Memory usage: ~1GB RAM

# License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

#Acknowledgments

- Oxford-IIIT Pets Dataset
- PyTorch and scikit-learn teams
  
