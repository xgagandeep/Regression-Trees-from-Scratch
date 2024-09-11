

# Project: Regression Trees from Scratch

**Date:** 2020  
**Language:** Python  
**Libraries:** NumPy, Matplotlib  
**Type:** Regression Tree Algorithm

## Description

This project implements regression trees from scratch using Python. It includes methods for creating, evaluating, and pruning regression trees. The project demonstrates a fundamental understanding of regression tree algorithms and their application for regression tasks.

## Features

- **Regression Tree Construction:** Builds a regression tree by recursively splitting data based on the best split criterion.
- **Data Splitting:** Splits the dataset into subsets based on feature values.
- **Tree Pruning:** Implements post-pruning to improve model performance by merging branches that do not provide significant improvements.
- **Forecasting:** Predicts outputs using the constructed regression tree.
- **Evaluation:** Computes and visualizes model performance using correlation coefficients and plots.

## Files

- **`Regression-Trees-from-Scratch.ipynb`:** Jupyter Notebook containing the implementation of regression trees from scratch.

## Installation

To run this project, you need Python and the required libraries installed. Follow these steps:

1. **Clone the repository:**

   ```bash
   git clone https://github.com/xgagandeep/Regression-Trees-from-Scratch.git
   ```

2. **Navigate to the project directory:**

   ```bash
   cd Regression-Trees-from-Scratch
   ```

3. **Install the required libraries:**

   ```bash
   pip install numpy matplotlib
   ```

4. **Run the Jupyter Notebook:**

   ```bash
   jupyter notebook Regression Trees from Scratch.ipynb
   ```

## Usage

1. **Data Preparation:** Provides sample training and testing datasets.
2. **Tree Creation:** Constructs a regression tree using the `create_tree` function.
3. **Tree Pruning:** Uses the `prune` function to prune the tree and avoid overfitting.
4. **Forecasting:** Predicts outputs on new data using the `treeForeCast` function.
5. **Evaluation:** Evaluates the model by computing correlation coefficients and visualizing results.

## Functions

- `regLeaf(dataset)`: Returns the mean of the target values for a given dataset.
- `regErr(dataset)`: Calculates the variance of the target values, scaled by the number of instances.
- `splitDataset(dataset, feature, value)`: Splits the dataset into two subsets based on the given feature and value.
- `create_tree(dataset, leafType, errType, ops)`: Constructs a regression tree recursively.
- `ChooseBestSplit(dataset, leafType, errType, ops)`: Finds the best split for the dataset based on error reduction.
- `prune(tree, testData)`: Prunes the tree using post-pruning techniques.
- `regTreeEval(model, inDat)`: Evaluates a regression tree model.
- `treeForeCast(tree, inData, modelEval)`: Forecasts output using the regression tree.
- `createForeCast(tree, testData, modelEval)`: Creates forecasts for test data.

## Performance

- **Tree Construction:** Builds a regression tree from scratch with custom splitting and evaluation functions.
- **Pruning:** Includes post-pruning to enhance model performance and prevent overfitting.
- **Visualization:** Provides plots to visualize the training data and model predictions.

## Contribution

Feel free to contribute to this project by submitting issues or pull requests. For any questions or feedback, please open an issue on the GitHub repository.
