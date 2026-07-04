# ML Learning Repository 🚀

A hands-on learning repository for exploring and mastering machine learning fundamentals using Python. This project focuses on data preprocessing, exploratory data analysis, and machine learning techniques.

## 📚 Project Overview

This repository serves as a practical learning hub for understanding core ML concepts including:
- **Data Loading & Exploration**: Working with datasets using Pandas and NumPy
- **Data Preprocessing**: Cleaning, encoding, and scaling features
- **Feature Engineering**: Handling missing values, encoding categorical variables
- **Data Imbalance**: Addressing class imbalance using oversampling techniques
- **Visualization**: Creating meaningful visualizations with Matplotlib

## 📁 Directory Structure

```
ML/
├── Learning basics of data sets.ipynb    # Main tutorial notebook for data fundamentals
├── sample.ipynb                          # Additional sample implementations
├── requirements.txt                      # Python dependencies
├── Datasets/                             # Raw datasets for learning
│   ├── adult/                           # Adult census income dataset
│   ├── heart+disease/                   # Heart disease prediction dataset
│   └── *.zip                            # Compressed datasets
├── data/                                # Processed/output data directory
├── models/                              # Saved models (if any)
└── README.md                            # This file
```

## 🛠️ Tech Stack

- **Python 3.x**
- **Pandas**: Data manipulation and analysis
- **NumPy**: Numerical computing
- **Scikit-learn**: Machine learning algorithms & preprocessing
  - StandardScaler for feature scaling
  - OneHotEncoder for categorical encoding
- **Imbalanced-learn**: Handling class imbalance with RandomOverSampler
- **Matplotlib**: Data visualization
- **Jupyter Notebook**: Interactive learning environment

## 📦 Installation

### Prerequisites
- Python 3.8 or higher
- pip or conda package manager

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone <repository-url>
   cd ML
   ```

2. **Create a virtual environment** (recommended)
   ```bash
   python -m venv .venv
   source .venv/bin/activate  # On Windows: .venv\Scripts\activate
   ```

3. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

## 🚀 Getting Started

1. **Launch Jupyter Notebook**
   ```bash
   jupyter notebook
   ```

2. **Start with the main tutorial**
   - Open `Learning basics of data sets.ipynb`
   - This notebook covers fundamental concepts in data preprocessing and analysis

3. **Explore datasets**
   - Navigate through the `Datasets/` directory
   - Each folder contains different datasets for learning

## 📊 Available Datasets

### Adult Dataset
- **Purpose**: Binary classification task (income prediction)
- **Size**: Multi-feature census data
- **Located in**: `Datasets/adult/`

### Heart Disease Dataset
- **Purpose**: Medical data analysis and prediction
- **Size**: Patient health metrics
- **Located in**: `Datasets/heart+disease/`

## 🔑 Key Concepts Covered

### Data Exploration
- Loading data with Pandas
- Understanding data structure and types
- Statistical summaries

### Data Cleaning & Preprocessing
- Handling missing values
- Removing duplicates
- Standardizing data types

### Feature Engineering
- **Encoding**: Converting categorical variables using OneHotEncoder
- **Scaling**: Normalizing numerical features with StandardScaler
- **Balancing**: Addressing class imbalance with RandomOverSampler

### Visualization
- Matplotlib for creating plots and charts
- Understanding data distributions
- Identifying patterns and outliers

## 💡 Usage Examples

```python
import pandas as pd
from sklearn.preprocessing import StandardScaler, OneHotEncoder
from imblearn.over_sampling import RandomOverSampler

# Load data
df = pd.read_csv('data.csv')

# Scale features
scaler = StandardScaler()
scaled_data = scaler.fit_transform(df)

# Handle class imbalance
ros = RandomOverSampler()
X_resampled, y_resampled = ros.fit_resample(X, y)
```

## 📝 Notebooks

- **Learning basics of data sets.ipynb**: Main tutorial covering:
  - Library imports and configuration
  - Data loading and exploration
  - Preprocessing workflows
  - Feature engineering techniques

- **sample.ipynb**: Additional examples and experiments

## 🎯 Learning Path

1. Start with basic imports and setup
2. Load and explore datasets
3. Understand data structure and statistics
4. Clean and preprocess data
5. Engineer features (encoding, scaling)
6. Address data imbalance
7. Visualize findings

## 🐛 Troubleshooting

- **Import errors**: Ensure all dependencies are installed with `pip install -r requirements.txt`
- **Dataset not found**: Verify datasets are in the `Datasets/` directory
- **Notebook kernel issues**: Restart the kernel or reinstall Jupyter

## 📚 Resources

- [Pandas Documentation](https://pandas.pydata.org/docs/)
- [Scikit-learn User Guide](https://scikit-learn.org/stable/user_guide.html)
- [NumPy Documentation](https://numpy.org/doc/)
- [Imbalanced-learn Documentation](https://imbalanced-learn.org/)

## 🤝 Contributing

This is a personal learning repository. Feel free to fork and adapt for your own learning!

## 📄 License

Open for educational purposes.

---

**Last Updated**: July 2026  
**Status**: 🚀 Active Learning
