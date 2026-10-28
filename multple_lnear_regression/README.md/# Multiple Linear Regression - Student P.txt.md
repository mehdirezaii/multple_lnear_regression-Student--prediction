# Multiple Linear Regression - Student Performance Prediction

A machine learning project that predicts students' academic performance using Multiple Linear Regression with Python and scikit-learn.

## Project Overview

This project implements a Multiple Linear Regression model to investigate the relationship between students' study habits, previous academic scores, and their performance index.

Unlike Simple Linear Regression, which uses a single input feature, this model uses multiple numerical features to predict a numerical target.

The project follows a basic machine learning workflow, including data loading, exploratory data analysis, visualization, training and testing data separation, model training, and performance evaluation.

## Objectives

- Explore and understand the Student Performance dataset.
- Select relevant numerical features for model training.
- Visualize relationships between individual features and the target variable.
- Implement Multiple Linear Regression using scikit-learn.
- Train the model on a training dataset and evaluate it on a separate test dataset.
- Interpret regression coefficients and the intercept.
- Evaluate model performance using Mean Squared Error (MSE) and R².

## Dataset

The project uses the **Student Performance** dataset.

The selected features are:

| Feature | Description |
|---|---|
| `Hours Studied` | Number of hours spent studying |
| `Previous Scores` | Previous academic scores |
| `Sleep Hours` | Number of hours spent sleeping |
| `Sample Question Papers Practiced` | Number of practice question papers completed |

**Target variable:**

- `Performance Index` - A numerical indicator of student performance.

The model uses the four selected input features to estimate the Performance Index.

## Technologies Used

- **Python** - Programming language
- **Jupyter Notebook** - Interactive development environment
- **NumPy** - Numerical computations
- **pandas** - Data manipulation and analysis
- **Matplotlib** - Data visualization
- **scikit-learn** - Machine learning and model evaluation

## Project Structure

```text
multiple-linear-regression-student-performance/
│
├── data/
│   └── Student_Performance.csv
│
├── notebook/
│   └── multiple_linear_regression.ipynb
│
├── README.md
├── requirements.txt
└── .gitignore
```

## Implementation Workflow

### 1. Data Loading and Exploration

- Load the dataset using pandas.
- Inspect sample records and descriptive statistics.
- Select the relevant input features and target variable.

### 2. Data Visualization

- Visualize the relationship between study hours and performance.
- Visualize the relationship between practice question papers and performance.
- Compare the distributions of training and test observations.

### 3. Train-Test Split

The dataset is divided into training and test subsets.

The training data is used to fit the model, while the test data is used to evaluate its performance on observations not used during training.

### 4. Model Training

The model is implemented using scikit-learn's `LinearRegression` class.

The input features are:

- Hours Studied
- Previous Scores
- Sleep Hours
- Sample Question Papers Practiced

The target variable is `Performance Index`.

### 5. Model Evaluation

The model is evaluated using Mean Squared Error (MSE) and the coefficient of determination (R²).

The current notebook reports the following results:

| Metric | Result |
|---|---:|
| Mean Squared Error (MSE) | 4.32 |
| R² Score | 0.99 |

**Note:** These are the results from the current notebook run. The exact values may vary depending on the random train-test split.

### Understanding the Results

- **MSE = 4.32:** The average squared difference between the model's predictions and the actual target values is 4.32, in squared target units.
- **R² = 0.99:** The model explains approximately 99% of the variance in the target values on the evaluated test data.

These results indicate a strong fit on this test split. However, they do not guarantee the same performance on every dataset or in real-world situations.

## Key Learning Outcomes

Through this project, I practiced:

- Working with a dataset containing multiple input features.
- Understanding the difference between Simple and Multiple Linear Regression.
- Selecting features and a target variable using pandas.
- Visualizing relationships between numerical variables.
- Splitting data into training and test subsets.
- Training a regression model with scikit-learn.
- Interpreting regression coefficients and the intercept.
- Evaluating predictions using MSE and R².
- Developing and documenting a machine learning project for GitHub.

## Installation and Usage

### 1. Clone the repository

```bash
git clone https://github.com/YOUR_USERNAME/multiple-linear-regression-student-performance.git
```

Replace `YOUR_USERNAME` with your GitHub username.

### 2. Navigate to the project directory

```bash
cd multiple-linear-regression-student-performance
```

### 3. Install dependencies

```bash
pip install -r requirements.txt
```

### 4. Open Jupyter Notebook

```bash
jupyter notebook
```

Open `notebook/multiple_linear_regression.ipynb` and run the cells in order.

Ensure that the dataset is available at the path expected by the notebook.

## Future Improvements

- Use a reproducible train-test split with `random_state`.
- Evaluate the model using Mean Absolute Error (MAE) and Root Mean Squared Error (RMSE).
- Compare the multiple regression model against a single-feature baseline.
- Examine residuals and potential model assumptions.
- Improve data loading so the notebook uses a project-relative path.
- Document the dataset source and license.

## Author

**Mehdi Rezaei**

Computer Engineering Student

Interested in Machine Learning, Artificial Intelligence, and Robotics.