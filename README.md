# Kryptonite-N

Coursework for Mathematics for Machine Learning (70015) at Imperial College London. 

This repository contains a collection of Jupyter Notebooks developed for the to solve the coursework task. Each notebook is designed to address a specific aspect of the project, from data analysis to model evaluation and sustainability considerations.

## Repository Structure

### Scripts  
The following scripts are the core components of this repository:

### 1. `data_analysis.ipynb`
- **Description:** 
  - This notebook contains the initial data exploration and analysis.
  - It includes data visualization, statistical summaries, and preprocessing steps to prepare the dataset for machine learning tasks.
- **Purpose:** Understand the dataset and identify patterns, correlations, and potential challenges.

### 2. `hyperparameter_tuning.ipynb`
- **Description:** 
  - Focuses on optimizing model performance by tuning hyperparameters using techniques like grid search, random search, or Bayesian optimization.
  - Includes experiments and results for different sets of hyperparameters.
- **Purpose:** Improve model performance by finding the best hyperparameter configuration.

### 3. `training_and_testing.ipynb`
- **Description:** 
  - Implements the training and testing of machine learning models.
  - Includes model evaluation metrics, such as accuracy, precision, recall, F1-score, and confusion matrices.
- **Purpose:** Train models on the dataset and evaluate their performance on unseen data.

### 4. `hidden_data_labels_generation.ipynb`
- **Description:** 
  - Contains methods to generate labels for hidden or unannotated data.
  - Uses techniques like semi-supervised learning, clustering, or heuristic labeling.
- **Purpose:** Augment the dataset by generating labels for unlabeled samples to expand the training data.

### 5. `other_models_explored.ipynb`
- **Description:** 
  - Documents experiments with additional machine learning models beyond the main approach.
  - Includes comparative analysis of their performance against the primary model.
- **Purpose:** Explore alternative modeling approaches and document insights.

### 6. `sustainability.ipynb`
- **Description:** 
  - Investigates the sustainability aspects of the project.
  - Includes analyses of model efficiency, energy consumption, and potential optimizations.
- **Purpose:** Ensure the project aligns with sustainable practices and minimizes environmental impact.

### Directories  
Apart from the scripts, this repository also contains the following directories:  

- **`Plots`**  
  - Contains all plots generated from the scripts.  
  - Organized by the corresponding notebook and analysis step.  

- **`Results`**  
  - Contains all numerical results obtained from various experiments.  
  - Includes hyperparameter optimization results, model evaluation metrics, and other statistics.  

- **`Datasets`**  
  - Contains the `Kryptonite-n` datasets used in the project.  
  - Includes raw, processed, and labeled datasets.

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
