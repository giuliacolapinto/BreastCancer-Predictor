# Breast Cancer Diagnostic Analysis

A comprehensive analysis using machine learning models for breast cancer diagnostic using the Breast Cancer Wisconsin (Diagnostic) dataset.

## 📋 Project Description

This project implements a complete machine learning pipeline to classify tumors as malignant or benign. The dataset contains 30 features derived from digitized images of breast biopsies and includes information on patients with diagnosed cancer.

**Objective**: Build a classification model capable of predicting with high accuracy whether a tumor is malignant (M) or benign (B).

## 📊 Dataset

- **Source**: UCI Machine Learning Repository - Breast Cancer Wisconsin (Diagnostic)
- **Number of samples**: 569
- **Number of features**: 30 (computed from 10 baseline characteristics)
- **Target**: Diagnosis (Malignant/Benign)

### Main features

The 30 features are derived from 10 baseline measurements:
- radius
- texture
- perimeter
- area
- smoothness
- compactness
- concavity
- concave points
- symmetry
- fractal dimension

For each characteristic, the following are computed: mean, standard error, and worst.

## 🚀 Quick Start

### Requirements

- Python 3.8+
- pip

### Installation

```bash
# Clone the repository
git clone https://github.com/[your-username]/breast-cancer-diagnostic-analysis.git
cd breast-cancer-diagnostic-analysis

# Create a virtual environment (recommended)
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate

# Install dependencies
pip install -r requirements.txt
```

### Usage

```bash
# Start the Jupyter notebook
jupyter notebook Notebook2.ipynb
```

## 📦 Dependencies

```
pandas>=1.3.0
numpy>=1.21.0
scikit-learn>=1.0.0
matplotlib>=3.4.0
seaborn>=0.11.0
jupyter>=1.0.0
ucimlrepo>=0.0.1
```

See `requirements.txt` for the full list.

## 📈 Project Structure

```
breast-cancer-diagnostic-analysis/
├── Notebook2.ipynb          # Main notebook with complete analysis
├── README.md                # This file
├── requirements.txt         # Project dependencies
└── .gitignore               # Files to ignore in Git
```

## 🔍 Analysis in the Notebook

The project includes:

1. **Dependency Installation**: Initial setup with `ucimlrepo`

2. **Data Loading**: Importing the dataset via UCI ML Repository
   - Manual definition of the 30 feature names
   - Removal of the ID column (not predictive)

3. **Exploratory Data Analysis (EDA)**:
   - Descriptive and statistical analysis
   - Data distribution visualization
   - Correlation analysis
   - Outlier identification

4. **Preprocessing**:
   - Data standardization/normalization
   - Handling missing values
   - Feature selection/engineering

5. **Modeling**:
   - Train/test splitting
   - Training different models (e.g., Logistic Regression, Random Forest, SVM, etc.)
   - Hyperparameter tuning

6. **Evaluation**:
   - Metrics: Accuracy, Precision, Recall, F1-Score
   - Confusion Matrix
   - ROC-AUC Curve

## 📊 Expected Results

The model should achieve high classification performance with an accuracy of over 95% on the test set.

## 💡 Technical Notes

- The `wdbc.data` file is headless, which is why features are defined manually
- Patient ID is removed as it's not a predictive feature
- Data is standardized prior to modeling

## 🤝 Contributions

Contributions are welcome! If you find bugs or have suggestions:

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📄 License

This project is licensed under the MIT License. See the `LICENSE` file for details.



**Note**: This project is for educational purposes only and should not be used for actual medical diagnoses.
