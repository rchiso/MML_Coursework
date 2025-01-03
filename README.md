# Kryptonite-N

Coursework for Mathematics for Machine Learning (70015) at Imperial College London. 

This repository contains a collection of Jupyter Notebooks developed for solving the coursework task. Each notebook is designed to address a specific aspect of the project, from data analysis to model evaluation and sustainability considerations.

The repository also includes our response paper, [`report.pdf`](./report.pdf), which disproves the claim that the Kryptonite-n dataset cannot be tackled with existing machine learning techniques.

## Repository Structure

### Scripts  
The following scripts are the core components of this repository:

### 1. [`data_analysis.ipynb`](./data_analysis.ipynb)
- **Description:** 
  - This notebook contains the initial data exploration and analysis.
  - This includes plots of histogram distribution of the features, singular values, principal component analysis, mutual information between features, etc.
  - Resulting plots are saved in [`Plots/DataAnalysis`](./Plots/DataAnalysis/)
- **Purpose:** Understand the dataset and identify patterns, and correlations.

### 2. [`hyperparameter_tuning.ipynb`](./hyperparameter_tuning.ipynb)
- **Description:** 
  - This notebook contains code to get validation accuracies (using K-fold validation) with different combinations of hyperparameters for different `Kryptonite-n` (n = 9, 12, 15) datasets.
  - The results of the experiments are stored in csv files in the directory [`Results/HyperparameterTuning`](./Results/HyperparameterTuning/).
  - The plots of validation accuracy achieved for different hyperparameter combinations are generated and stored as svg files in the directory [`Plots/HyperparameterTuning`](./Plots/HyperparameterTuning/).
- **Purpose:** Improve model performance by finding the best hyperparameter configuration.

### 3. [`mlp.ipynb`](./mlp.ipynb)
- **Description:** 
  - Trains and tests MLP model for different `Kryptonite-n` (n = 9, 12, 15) datasets (using the selected hyperparamaters).
  - Plots the mean and standard deviation in test accuracies over multiple training runs.
  - Generates the labels for the hidden Kryptonite datesets.
  - Results and plots are saved in [`Results/MLPTrainingAndTesting`](./Results/MLPTrainingAndTesting) and [`Plots/MLPTrainingAndTesting`](./Plots/MLPTrainingAndTesting) respectively.
- **Purpose:** Solve the dataset with acceptable accuracy using MLP.

### 4. [`svm.ipynb`](./svm.ipynb)
- **Description:** 
  - Trains and tests SVM model for different `Kryptonite-n` (n = 9, 12, 15) datasets.
  - Calculate and plot training and test accuracy results.
  - Results are saved in [`Results/SVMTrainingAndTesting`](./Results/SVMTrainingAndTesting/), and [`Plots/SVMTrainingAndTesting`](./Plots/SVMTrainingAndTesting/).
- **Purpose:** Provide different comparable ML model training for main approach (MLP).

### 5. [`model_comparison.ipynb`](./model_comparison.ipynb)
- **Description:** 
  - This script compares the results of MLP and SVM.
  - Plots are saved in [`Plots/ModelComparison`](./Plots/ModelComparison).
- **Purpose:** Select the best model.

### 6. [`sustainability.ipynb`](./sustainability.ipynb)
- **Description:** 
  - Calculate and summarize model training's energy usage and its equivalent carbon emissions using different tools.
  - Calculate trained model's bias and fairness using different metrics.
  - Results are saved in [`Results/Sustainability/`](./Results/Sustainability/).
- **Purpose:** Analyzes the model's environmental, ethical, and societal impact.

### Directories  
Apart from the scripts, this repository also contains the following directories:  

- **[`Datasets`](./Datasets/)**: Contains the `Kryptonite-n` datasets used in the project.  

- **[`HiddenLabels`](./hiddenlabels/)**: Contains the predicted labels for the hidden Kryptonite-n datasets.

- **[`Model`](./model/)**: Contains the saved model parameters of the MLP used for generating the final predicted labels.

- **[`Plots`](./Plots/)**: Contains all plots generated from the scripts organized by the corresponding notebook.  

- **[`Results`](./Results/)**: Contains the numerical results data obtained from any experiments.

## Getting Started

### Prerequisites
- Python 3.x
- Jupyter Notebook
- Required Python packages (listed in `requirements.txt`)

### Installation
1. Clone this repository:
   ```bash
   git clone https://github.com/rchiso/MML_Coursework.git
   cd MML_Coursework
   ```

2. Install the dependencies
    ```bash
    pip install requirements.txt
    ```

3. You are now all set to run any of the scripts using Jupyter or any other IDE which supports running ipynb files.
