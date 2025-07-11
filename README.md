⚓ Titanic Survival Prediction  
This notebook builds machine learning models to predict passenger survival on the Titanic, applying data preprocessing and machine learning techniques to predict survival outcomes.

🗂️ Table of Contents  
- [💻 Installation](#installation)  
- [🎯 Project Goals](#project-goals)  
- [🧪 Methods](#methods)  
- [📈 Results](#results)  
- [🧾 Project Details](#project-details)  
- [🪪 License](#license)  

## 💻 Installation  
Requirements: Python 3.8+, Jupyter Notebook

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

## 🎯 Project Goals
- **Objective**: Predict whether a passenger survived the Titanic disaster using demographic and ticketing information.
- **Features Used**: Age, Sex, Passenger Class, Fare, Embarkation Port, Family Size (SibSp + Parch)
- **Target**: Binary classification (Survived: Yes/No)

## 🧪 Methods

### Models Used:
- 🌳 Decision Tree
- 🌲 Random Forest
- ⚡ XGBoost

### Techniques Applied:
- 🔤 Label encoding for categorical features (Sex, Embarked)
- 📊 MinMax scaling for numerical features
- 🧮 Feature engineering and selection
- 📋 Evaluation using precision, recall, F1-score
- 📊 Confusion matrices for visualization

## 📈 Results

| Model | Accuracy | Precision | Recall | F1-Score |
|-------|----------|-----------|---------|-----------|
| ⚡ XGBoost | 81.56% | 0.81 | 0.82 | 0.81 |
| 🌳 Decision Tree | 82.12% | 0.83 | 0.82 | 0.81 |
| 🌲 Random Forest | 79.33% | 0.80 | 0.79 | 0.78 |

🔎 **Key Insights**:
- Decision Tree showed the best overall performance with 82.12% accuracy
- All models demonstrated good balance between precision and recall
- Models performed well in identifying both survivors and non-survivors

## 🧾 Project Details
- **Notebook Structure**:
  - Data Preprocessing
  - Exploratory Data Analysis
  - Feature Engineering
  - Model Training & Evaluation
  - Results Comparison
- **Dataset**: titanic-passengers.csv (included in repository)
- **Dependencies**: All required packages listed in requirements.txt

## 🪪 License
This project is for educational and non-commercial use only.  
Dataset source: [Kaggle Titanic Dataset](https://www.kaggle.com/c/titanic) 