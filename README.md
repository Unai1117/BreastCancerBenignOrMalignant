# Tumor Prediction with Machine Learning

This project leverages machine learning algorithms to predict whether a tumor is benign or malignant using biomedical data. Various classification models are explored, and the best-performing model is selected based on its performance.

## Project Overview

The project follows these steps:

1. **Data Loading**: Downloading the dataset from OpenML.
2. **Data Exploration and Preparation**:
   - Analyzing dataset dimensions.
   - Assigning descriptive names to columns.
   - Visualizing the distribution of target classes.
3. **Model Training**:
   - Training and evaluating several classification models:
     - Random Forest
     - Logistic Regression
     - Support Vector Machine (SVM)
     - Gradient Boosting
   - Cross-validation to compare model performance.
4. **Hyperparameter Tuning**:
   - Using `GridSearchCV` to optimize hyperparameters of the Gradient Boosting model, selected as the best-performing model.

## Requirements

To run the project, you need the following dependencies:

- Python 3.7+
- Python libraries:
  - `openml`
  - `pandas`
  - `numpy`
  - `scikit-learn`
  - `seaborn`
  - `matplotlib`

Install the dependencies using:
```bash
pip install openml pandas numpy scikit-learn seaborn matplotlib
```

## Notebook Structure

The project is documented in a Jupyter notebook. The main structure includes:

1. **Introduction**: Brief description of the problem and objectives.
2. **Data Loading and Exploration**:
   - Loading the dataset from OpenML.
   - Initial exploratory analysis (dimensions, data types, class distribution).
3. **Model Training and Evaluation**:
   - Comparing different models using metrics such as `precision`, `recall`, and `F1-score`.
   - Visualizing results with plots.
4. **Best Model Optimization**:
   - Hyperparameter tuning with GridSearchCV to improve the accuracy of the Gradient Boosting model.
5. **Conclusions**: Summary of results and future steps.

## Usage

Follow these steps to run the notebook:

1. Clone the repository:
   ```bash
   git clone https://github.com/Unai1117/BreastCancerBenignOrMalignant.git
   ```

2. Navigate to the project directory:
   ```bash
   cd project_name
   ```

3. Open the notebook in Jupyter:
   ```bash
   jupyter notebook tumor_prediction.ipynb
   ```

4. Execute the cells sequentially to reproduce the analysis and results.

## Results

The optimized model (Gradient Boosting) achieved the following results:

- **Key Metrics**:
  - Accuracy: 98%
  - Recall: 97%
  - F1-Score: 97%

Detailed insights can be found in the hyperparameter tuning section and the classification reports generated by the models.

## Contributions

Contributions are welcome. To improve the project or add new features, follow these steps:

1. Fork the repository.
2. Create a branch for your feature:
   ```bash
   git checkout -b new_feature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Description of changes"
   ```
4. Push your changes and submit a pull request.

## License

This project is licensed under the MIT License. See the `LICENSE` file for more information.

