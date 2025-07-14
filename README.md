# ⚓ Titanic Survival Prediction

This notebook builds machine learning models to predict passenger survival on the Titanic, applying SMOTE (Synthetic Minority Oversampling Technique) to handle class imbalance and improve detection of survivors.

---

## 📚 Table of Contents

- [💻 Installation](#-installation)
- [🎯 Project Goals](#-project-goals)
- [🧪 Methods](#-methods)
- [📈 Results](#-results)
- [🧾 Project Details](#-project-details)
- [🪪 License](#-license)

---

## 💻 Installation

- **Requirements:** Python 3.8+, Jupyter Notebook

```bash
# Clone the repository
git clone https://github.com/alhussienhazem/titanic-survival-prediction.git

# Navigate to the project folder
cd titanic-survival-prediction

# (optional) create a virtual environment
python -m venv venv
source venv/bin/activate  # on Linux/Mac
venv\Scripts\activate     # on Windows

# Install dependencies
pip install -r requirements.txt

# Run the notebook
jupyter notebook
```

---

## 🎯 Project Goals

- **Objective:** Predict whether a passenger survived the Titanic disaster using demographic and ticketing information
- **Challenge:** Imbalanced dataset with fewer survivors (minority class)
- **Solution:** Apply SMOTE to oversample the minority class during training and improve recall
- **Features Used:** Age, Sex, Passenger Class, Fare, Embarkation Port, Family Size (SibSp + Parch)
- **Target:** Binary classification (Survived: Yes/No)

---

## 🧪 Methods

- **Models Used:**
  - 🌳 Decision Tree
  - 🌲 Random Forest
  - ⚡ XGBoost

- **Techniques Applied:**
  - 🔤 Label encoding for categorical features (Sex)
  - 📊 One-hot encoding for Embarked column
  - 📊 MinMax scaling for numerical features
  - 🧬 SMOTE to balance survival classes
  - 🧮 Feature engineering and selection
  - 📋 Evaluation using precision, recall, F1-score
  - 📊 Confusion matrices for visualization
  - 🔍 Duplicate removal and data validation

---

## 📈 Results

### **Original Model Performance**
| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|---------|-----------|
| 🌳 Decision Tree | 80.45% | 0.86 | 0.55 | 0.67 |
| 🌲 Random Forest | 81.01% | 0.84 | 0.58 | 0.69 |
| ⚡ XGBoost | 81.56% | 0.81 | 0.65 | 0.72 |

### **SMOTE Enhanced Performance**
| Model | Original Accuracy | With SMOTE | Improvement |
|-------|------------------|------------|-------------|
| 🌳 Decision Tree | 80.45% | 81.56% | +1.11% |
| 🌲 Random Forest | 81.01% | 81.01% | No change |
| ⚡ XGBoost | 81.56% | 82.12% | +0.56% |

### **Detailed Performance Metrics (with SMOTE):**
| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|---------|-----------|
| 🌳 Decision Tree | 81.56% | 0.84 | 0.88 | 0.86 |
| 🌲 Random Forest | 81.01% | 0.83 | 0.89 | 0.86 |
| ⚡ XGBoost | 82.12% | 0.84 | 0.89 | 0.86 |

### **Key Insights:**
- **SMOTE Implementation**: Successfully improved model performance, especially for Decision Tree (+1.11% accuracy)
- **Best Overall Performance**: XGBoost with SMOTE achieved 82.12% accuracy
- **Class Balance**: SMOTE helped improve detection of survivors (minority class)
- **Robust Evaluation**: All models demonstrated good balance between precision and recall
- **Recall Improvement**: Significant improvement in survivor detection across all models

---

## 🧾 Project Details

- **Enhanced Data Preprocessing:**
  - Duplicate removal and validation
  - Improved missing value handling
  - Enhanced feature encoding (one-hot encoding)
- **SMOTE Implementation:**
  - Applied to training data to balance classes
  - Improved minority class detection
  - Before/after performance comparison
- **Comprehensive Evaluation:**
  - Detailed classification reports
  - Confusion matrix visualizations
  - Multiple performance metrics
- **Notebook Structure:**
  - Data Preprocessing & Validation
  - Exploratory Data Analysis
  - Feature Engineering
  - SMOTE Application
  - Model Training & Evaluation
  - Results Comparison

---

## 🪪 License

This project is for educational and non-commercial use only.  
Dataset source: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic) 
