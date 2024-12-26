
# Compare Runs, Choose a Model, and Deploy it to a REST API

This project demonstrates a comprehensive workflow for building, tracking, and deploying an Artificial Neural Network (ANN) model using MLflow. It includes model experimentation, evaluation, and serving through a REST API.

## Table of Contents

1. [Project Overview](#project-overview)
2. [Features](#features)
3. [Technologies Used](#technologies-used)
4. [Installation](#installation)
5. [Usage](#usage)
6. [Workflow](#workflow)
7. [License](#license)

## Project Overview

The project focuses on the lifecycle of a machine learning model, particularly:
- Experimenting with various ANN configurations to optimize performance.
- Tracking experiments using MLflow to manage and compare runs.
- Selecting the best model based on performance metrics.
- Deploying the chosen model to a REST API for real-world usability.

This is ideal for tasks requiring model reproducibility, tracking, and scalable deployment.

## Features

- **Experiment Tracking:** Use MLflow to log and visualize training runs.
- **Model Evaluation:** Calculate metrics such as Mean Squared Error (MSE) to compare models.
- **Production Deployment:** Serve the trained model via a REST API.
- **Input Validation:** Ensure robust input handling in the API.

## Technologies Used

The following libraries and frameworks are used in this project:

- **MLflow**: For experiment tracking and deployment.
- **Keras**: For building and training the ANN model.
- **NumPy**: For numerical computations.
- **Pandas**: For data preprocessing.
- **Scikit-learn**: For splitting data into training and testing sets.
- **REST API**: For serving the deployed model.

## Installation

### Prerequisites

- Python 3.10 
- pip or conda for package management

### Steps

1. Clone this repository:
   ```bash
   git clone https://github.com/sushantrajbhar/ANN-Experimentation-with-MLflow.git
   cd ANN-Experimentation-with-MLflow
   ```

2. Create a virtual environment and activate it:
   ```bash
   python -m venv venv
   source venv/bin/activate  # On Windows: venv\Scripts\activate
   ```

3. Install required packages:
   ```bash
   pip install -r requirements.txt
   ```

4. Set up MLflow for local tracking.

## Usage

1. **Run the Notebook**:
   Execute the notebook to train and evaluate ANN models. MLflow will automatically log the runs.

2. **Deploy the Best Model**:
   Follow the notebook steps to register and deploy the best-performing model to a REST API.

3. **Test the REST API**:
   Use tools like Postman or curl to interact with the API.

## Workflow

1. **Data Preprocessing**:
   - Load and preprocess the dataset.
   - Split the data into training and testing sets using `train_test_split`.

2. **Model Training**:
   - Define and train an ANN using Keras.
   - Log model parameters, metrics, and artifacts to MLflow.

3. **Experiment Tracking**:
   - Compare model performance metrics like MSE across different runs.

4. **Model Deployment**:
   - Register the best model in MLflow.
   - Deploy it to a REST API.

5. **Input Validation and Testing**:
   - Validate input schema and ensure correct inference.

Do checkout the snapshots of MLFLOW UI under MLFLOW folder to know more about MLFLOW.

## License

This project is licensed under the MIT License. See the LICENSE file for details.
