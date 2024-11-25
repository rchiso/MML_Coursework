# Kryptonite-N

Coursework for Mathematics for Machine Learning (70015) at Imperial College London. 

This repository contains a collection of Jupyter Notebooks developed for solving the coursework task. Each notebook is designed to address a specific aspect of the project, from data analysis to model evaluation and sustainability considerations.

## Repository Structure

### Scripts  
The following scripts are the core components of this repository:

### 1. [`data_analysis.ipynb`](./data_analysis.ipynb)
- **Description:** 
  - It includes data visualization, statistical summaries, and preprocessing steps to prepare the dataset for machine learning tasks.
  - Resulting plots are saved in [./Plots/DataAnalysis/](./Plots/DataAnalysis/)
- **Purpose:** Understand the dataset and identify patterns, correlations, and potential challenges.

### 2. [`hyperparameter_tuning.ipynb`](./hyperparameter_tuning.ipynb)
- **Description:** 
  - This notebook contains code to get validation accuracies (using K-fold validation) with different combinations of hyperparameters for different `Kryptonite-n` (n = 9, 12, 15) datasets.
  - The results of the experiments are stored in csv files in the directory `Results/HyperparameterTuning`.
  - The plots of validation accuracy achieved for different hyperparameter combinations are generated and stored as svg files in the directory `Plots/HyperparameterTuning`.
- **Purpose:** Improve model performance by finding the best hyperparameter configuration.

### 3. [`training_and_testing.ipynb`](./training_and_testing.ipynb)
- **Description:** 
  - Implements the training and testing of machine learning models.
  - Includes model evaluation metrics, such as accuracy, precision, recall, F1-score, and confusion matrices.
- **Purpose:** Train models on the dataset and evaluate their performance on unseen data.

### 4. [`svm.ipynb`](./svm.ipynb)
- **Description:** 
  - Trains and tests SVM model for different `Kryptonite-n` (n = 9, 12, 15) datasets.
  - Calculate and plot training and test accuracy. Results are saved in [Results/SVMTrainingAndTesting](./Results/SVMTrainingAndTesting/), and [Plots/SVMTrainingAndTesting](./Plots/SVMTrainingAndTesting/).
- **Purpose:** Provide different ML approach(SVM) for solving the Kryptonite-n dataset.

### 4. [`model_comparison.ipynb`](./model_comparison.ipynb)
- **Description:** 
  - This script compares the results of MLP and SVM.
- **Purpose:** Select the best model

### 6. [`hidden_data_labels_generation.ipynb`]()
- **Description:** 
  - Contains methods to generate labels for hidden or unannotated data.
  - Uses techniques like semi-supervised learning, clustering, or heuristic labeling.
- **Purpose:** Augment the dataset by generating labels for unlabeled samples to expand the training data.

### 7. [`sustainability.ipynb`](./sustainability.ipynb)
- **Description:** 
  - Calculate and summarize model training's energy usage and its equivalent carbon emissions using different tools. Results are saved in [Results/Sustainability/](./Results/Sustainability/)
  - Calculate trained model's bias and fairness using different metrics. Results are also saved in [Results/Sustainability/](./Results/Sustainability/)
- **Purpose:** Analyzes the model's environmental, ethical, and societal impact.

### Directories  
Apart from the scripts, this repository also contains the following directories:  

- **`Plots`**: Contains all plots generated from the scripts organized by the corresponding notebook.  

- **`Results`**: Contains the numerical results data obtained from any experiments.

- **`Datasets`**: Contains the `Kryptonite-n` datasets used in the project.  

- **`HiddenLabels`**: Contains the predicted labels for the hidden Kryptonite-n datasets.

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
