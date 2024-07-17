# Mental-health-prediction-using-Machine-Learning

## Table of Contents
1. [Introduction](#introduction)
2. [Dataset](#dataset)
3. [Data Preprocessing](#data-preprocessing)
4. [Modeling](#modeling)
5. [Evaluation](#evaluation)
6. [Usage](#usage)
7. [Requirements](#requirements)
8. [Contributing](#contributing)
9. [License](#license)

## Introduction
This project aims to predict mental health treatment needs based on various factors such as age, gender, work environment, and more. The dataset is derived from a survey about mental health in the tech workplace.

## Dataset
The dataset used for this project is `survey.csv`, which contains responses from individuals about their mental health and workplace conditions.

### Data Columns:
- Age
- Gender
- Country
- Self-employed
- Family history
- Treatment
- Work interfere
- No employees
- Remote work
- Tech company
- Benefits
- Care options
- Wellness program
- Seek help
- Anonymity
- Leave
- Mental health consequence
- Physical health consequence
- Coworkers
- Supervisor
- Mental health interview
- Physical health interview
- Mental vs. physical
- Observed consequence
- Comments

## Data Preprocessing
The following preprocessing steps were applied to the dataset:
1. **Missing Data Handling**: Columns with significant missing values such as `comments`, `state`, and `Timestamp` were dropped. Remaining NaN values were filled with default values based on the data type.
2. **Gender Cleaning**: Standardized gender values to `male`, `female`, and `trans`. Removed non-relevant entries.
3. **Feature Selection**: Selected relevant features for modeling.

## Modeling
Various machine learning models were implemented using `scikit-learn`:
1. **Logistic Regression**
2. **Decision Tree Classifier**
3. **Random Forest Classifier**
4. **Extra Trees Classifier**
5. **Neural Network (MLPClassifier)**
6. **Bagging Classifier**
7. **AdaBoost Classifier**
8. **K-Neighbors Classifier**
9. **Gaussian Naive Bayes**
10. **Stacking Classifier** using `mlxtend`

## Evaluation
The models were evaluated using the following metrics:
- Accuracy Score
- Precision-Recall Curve
- Cross-Validation Score

## Usage
To run the project, follow these steps:
1. Clone the repository.
   ```bash
   git clone https://github.com/your-username/mental-health-prediction.git
   cd mental-health-prediction
   ```
2. Install the required libraries.
   ```bash
   pip install -r requirements.txt
   ```
3. Upload the dataset `survey.csv` to the project directory.
4. Run the preprocessing and modeling script.
   ```bash
   python main.py
   ```

## Requirements
- Python 3.7+
- `numpy`
- `pandas`
- `matplotlib`
- `seaborn`
- `scikit-learn`
- `mlxtend`

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
