# Cat vs Dog Image Classification using CNN

**Deep Learning Project: Binary Image Classification with TensorFlow and Keras**

<div align="center">

![TensorFlow](https://img.shields.io/badge/TensorFlow-FF6F00?style=for-the-badge&logo=tensorflow&logoColor=white)
![Keras](https://img.shields.io/badge/Keras-D00000?style=for-the-badge&logo=keras&logoColor=white)
![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)
![Jupyter](https://img.shields.io/badge/Jupyter-F37626?style=for-the-badge&logo=jupyter&logoColor=white)

</div>

---

## 📋 Overview

This project implements a **Convolutional Neural Network (CNN)** for binary image classification to distinguish between cats and dogs. Built using TensorFlow and Keras, it demonstrates a complete deep learning workflow from data preprocessing to model evaluation.

The model is trained on the popular **Kaggle Cats and Dogs dataset** containing 25,000 labeled images, providing hands-on experience with computer vision and deep learning techniques.

---

## 🎯 Problem Statement

Image classification is a fundamental computer vision task with applications in medical imaging, autonomous vehicles, security systems, and more. This project tackles the binary classification challenge: given an image, determine whether it contains a cat or a dog.

**Challenges Addressed:**
- Handling large image datasets efficiently
- Data preprocessing and augmentation
- CNN architecture design for image recognition
- Model training and hyperparameter tuning
- Evaluation and performance metrics

---

## 🚀 Objectives

1. **Data Preprocessing**: Load and prepare 25,000 images for training
2. **Model Architecture**: Design and implement a CNN for binary classification
3. **Training**: Train the model with appropriate hyperparameters
4. **Evaluation**: Assess model performance using accuracy metrics and validation data
5. **Visualization**: Display training progress, predictions, and model insights

---

## ✨ Features

- ✅ Complete ML pipeline implementation
- ✅ Data loading and preprocessing
- ✅ Image data augmentation
- ✅ CNN architecture with multiple convolutional and pooling layers
- ✅ Model training with validation split
- ✅ Performance visualization (accuracy, loss curves)
- ✅ Model evaluation on test data
- ✅ Jupyter Notebook with detailed documentation

---

## 🛠️ Technologies Used

### Core Frameworks
- **TensorFlow 2.18.0** - Deep learning framework
- **Keras 3.8.0** - High-level neural networks API
- **Python 3.x** - Programming language

### Data Science Libraries
- **NumPy** - Numerical computations
- **Pandas** - Data manipulation
- **Matplotlib** - Data visualization
- **Seaborn** - Statistical visualizations
- **Pillow** - Image processing

---

## 📊 Dataset

**Source:** Kaggle Cats and Dogs Dataset  
**Size:** 25,000 images (12,500 cats + 12,500 dogs)  
**Format:** JPEG images of various sizes  
**Split:** Training and validation sets

The dataset provides a balanced binary classification problem with real-world image variations in:
- Lighting conditions
- Image quality
- Pet positions and angles
- Background complexity

---

## 🏗️ Model Architecture

### CNN Structure

The model uses a sequential Convolutional Neural Network with the following layers:

1. **Convolutional Layers**: Feature extraction from images
2. **Pooling Layers**: Spatial dimension reduction
3. **Flatten Layer**: Convert 2D features to 1D
4. **Dense Layers**: Fully connected layers for classification
5. **Output Layer**: Binary classification (Sigmoid activation)

**Key Architectural Decisions:**
- Multiple conv-pool blocks for hierarchical feature learning
- ReLU activation for non-linearity
- Dropout for regularization (if implemented)
- Binary crossentropy loss for binary classification

---

## 💻 Installation

### Prerequisites

- Python 3.8 or higher
- Jupyter Notebook or JupyterLab
- pip package manager

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/zohaibsumbal786/cat-and-dog-classification.git
   cd cat-and-dog-classification
   ```

2. **Install required dependencies**
   ```bash
   pip install tensorflow==2.18.0 keras==3.8.0 numpy pandas matplotlib seaborn pillow
   ```

3. **Download the dataset**
   - Download from [Kaggle Cats and Dogs Dataset](https://www.kaggle.com/c/dogs-vs-cats/data)
   - Extract to a local directory
   - Update the dataset path in the notebook

4. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook Untitled141.ipynb
   ```

---

## 📁 Project Structure

```
cat-and-dog-classification/
│
├── Untitled141.ipynb              # Main Jupyter notebook with complete workflow
├── Dog_vs_Cat_Classification_Report.docx  # Project report and analysis
├── README.md                      # This file
├── .gitignore                     # Git ignore configuration
│
└── data/                          # Dataset directory (not included in repo)
    ├── train/
    │   ├── cats/
    │   └── dogs/
    └── test/
```

---

## 🔄 Usage

### Running the Notebook

1. Open `Untitled141.ipynb` in Jupyter Notebook
2. Update the dataset path to your local directory
3. Run cells sequentially:
   - **Data Loading**: Import and inspect the dataset
   - **Preprocessing**: Resize images, normalize pixel values
   - **Model Definition**: Build the CNN architecture
   - **Training**: Train the model (10 epochs default)
   - **Evaluation**: Validate performance on test data
   - **Visualization**: View accuracy/loss curves and predictions

### Training Configuration

```python
# Default hyperparameters
EPOCHS = 10
BATCH_SIZE = 32
IMAGE_SIZE = (150, 150)  # Target image dimensions
VALIDATION_SPLIT = 0.2
```

Adjust these parameters in the notebook for experimentation.

---

## 📈 Results and Demonstration

### Training Progress

The model was trained for **10 epochs** with the following observations:

- **Training Accuracy**: Progressively improved across epochs
- **Validation Accuracy**: Monitored to detect overfitting
- **Loss Curves**: Visualized training and validation loss

### Model Performance

Results include:
- Accuracy metrics on training and validation sets
- Confusion matrix for classification performance
- Sample predictions with confidence scores

*Note: Specific accuracy values can be found in the notebook execution output and the project report.*

### Visualizations

The notebook includes:
- Training/validation accuracy curves
- Training/validation loss curves
- Sample image predictions with true vs predicted labels
- Model architecture summary

---

## 🔮 Future Improvements

1. **Model Enhancements**
   - Experiment with deeper architectures (ResNet, VGG, EfficientNet)
   - Implement transfer learning with pre-trained models
   - Add batch normalization and dropout for regularization
   - Try data augmentation (rotation, zoom, flip)

2. **Performance Optimization**
   - Hyperparameter tuning with grid search
   - Learning rate scheduling
   - Early stopping to prevent overfitting
   - Class weight balancing if needed

3. **Deployment**
   - Convert model to TensorFlow Lite for mobile deployment
   - Build a web interface for real-time predictions
   - Create a REST API for model serving
   - Deploy to cloud platforms (AWS, GCP, Azure)

4. **Extended Functionality**
   - Multi-class classification (add more animal types)
   - Object detection (localize cats/dogs in images)
   - Breed classification within cats and dogs
   - Real-time video classification

---

## 📚 Learning Outcomes

This project demonstrates practical skills in:
- ✅ Convolutional Neural Networks (CNNs)
- ✅ Image preprocessing and augmentation
- ✅ Deep learning model training and evaluation
- ✅ TensorFlow and Keras framework usage
- ✅ Computer vision fundamentals
- ✅ Binary classification problems
- ✅ Model performance visualization
- ✅ Jupyter Notebook for reproducible research

---

## 🤝 Contributing

Contributions are welcome! If you'd like to improve this project:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/improvement`)
3. Commit your changes (`git commit -m 'Add some improvement'`)
4. Push to the branch (`git push origin feature/improvement`)
5. Open a Pull Request

---

## 📄 License

This project is open source and available for educational purposes.

---

## 👤 Author

**Zohaib Ahmed Khan Sumbal**

- GitHub: [@zohaibsumbal786](https://github.com/zohaibsumbal786)
- LinkedIn: [Connect with me](#)

---

## 🙏 Acknowledgments

- **Kaggle** for providing the Cats and Dogs dataset
- **TensorFlow and Keras** teams for excellent deep learning frameworks
- **Python community** for comprehensive data science libraries

---

<div align="center">

### 🐱🐶 Happy Classifying! 

*Built with passion for AI and computer vision*

</div>
