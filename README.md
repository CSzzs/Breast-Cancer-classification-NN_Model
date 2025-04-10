# Breast Cancer Classification using Neural Networks

A deep learning model to classify breast cancer tumors as either Malignant or Benign using the Wisconsin Breast Cancer dataset.

## Project Overview
This project implements a neural network classifier to detect breast cancer using various cell nucleus characteristics. The model achieves high accuracy in distinguishing between malignant and benign tumors.

## Dataset
The project uses the [Breast Cancer Wisconsin (Diagnostic) Dataset](https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data) from Kaggle which includes features computed from a digitized image of a fine needle aspirate (FNA) of a breast mass.

### Features Include:
- Radius
- Texture
- Perimeter
- Area
- Smoothness
- Compactness
- Concavity
- Symmetry
- Fractal dimension

## Project Structure
1. Data Preprocessing
   - Loading and cleaning the dataset
   - Removing unnecessary columns
   - Label encoding for diagnosis
   - Feature standardization

2. Exploratory Data Analysis (EDA)
   - Statistical analysis
   - Distribution plots
   - Correlation matrix visualization
   - Outlier detection using box plots

3. Model Architecture
   - Input layer (30 features)
   - Hidden layer with 20 neurons (ReLU activation)
   - Output layer with 2 neurons (Sigmoid activation)

## Requirements
```python
numpy
pandas
matplotlib
seaborn
sklearn
tensorflow
opendatasets
```

## Model Performance
- The model is trained for 10 epochs
- Uses Adam optimizer
- Loss function: sparse categorical crossentropy
- Includes validation split for monitoring training

## Usage
1. Install dependencies:
```bash
pip install -r requirements.txt
```

2. Download the dataset using:
```python
import opendatasets as od
od.download('https://www.kaggle.com/datasets/uciml/breast-cancer-wisconsin-data')
```

3. Run the notebook to:
   - Perform data analysis
   - Train the model
   - Make predictions

## Predictive System
The notebook includes a prediction system that can classify new tumor samples. Input should be a tuple of 30 features corresponding to the tumor characteristics.

## Visualizations
The project includes various visualizations:
- Feature distributions
- Correlation heatmap
- Training and validation accuracy curves
- Training and validation loss curves
- Box plots for outlier detection

## Results
The model achieves high accuracy in classifying breast cancer tumors, making it a useful tool for medical diagnosis support.

## License
This project is open source and available under the MIT License.

## Contributing
Feel free to fork this repository and submit pull requests to contribute to this project.

## Acknowledgments
- UCI Machine Learning Repository
- Wisconsin Breast Cancer Dataset contributors
- Kaggle for hosting the dataset
