# Support Vector Machine Tutorial

## Overview
This project is a tutorial on implementing Support Vector Machines (SVM) for classification using Python and scikit-learn. It uses the Iris dataset to demonstrate how to train SVM models with different kernels (RBF, Polynomial, Linear) and evaluate their performance.

## Dataset
The Iris dataset is loaded from `sklearn.datasets.load_iris()`. It contains:
- 150 samples
- 4 features: sepal length, sepal width, petal length, petal width (all in cm)
- 3 target classes: setosa (0), versicolor (1), virginica (2)

## Project Structure
- **Support Vector Machine.ipynb**: Jupyter notebook containing the tutorial code for data loading, exploration, model training, and evaluation.

## Prerequisites
To run the notebook, install the required Python libraries:
```bash
pip install pandas scikit-learn matplotlib seaborn
```

## Steps in the Notebook
1. **Data Loading**:
   - Load the Iris dataset using `load_iris()` from scikit-learn.
   - Create a pandas DataFrame with features and add the target column.

2. **Data Exploration**:
   - Map target values to flower names for better readability.
   - Perform groupby operations to calculate mean values for each class.
   - Visualize data using scatter plots for different feature pairs colored by class.

3. **Data Splitting**:
   - Split the data into features (X) and target (y).
   - Use `train_test_split` to create training (80%) and testing (20%) sets.

4. **Model Training and Evaluation**:
   - Train SVM with default RBF kernel and evaluate on test set.
   - Train SVM with Polynomial kernel.
   - Train SVM with Linear kernel.

## Results
- SVM with RBF kernel: Test accuracy ~0.9667
- SVM with Polynomial kernel: Test accuracy ~0.9667
- SVM with Linear kernel: Test accuracy ~0.9667
The models perform similarly well on the Iris dataset due to its simplicity.

## How to Run
1. Clone this repository:
   ```bash
   git clone <repository-url>
   ```
2. Open the Jupyter notebook:
   ```bash
   jupyter notebook 08_Support_Vector_Machine.ipynb
   ```
3. Run all cells to reproduce the tutorial and results.

## License
This project is licensed under the MIT License.
