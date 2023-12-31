# Financial Predictive Analytics

This project aims to predict financial market trends and stock prices using machine learning models and historical stock data.

## Table of Contents

- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
- [Data Sources](#data-sources)
- [Model Explanation](#model-explanation)
- [Model Performance](#model-performance)
- [Usage Instructions](#usage-instructions)
- [Contributing](#contributing)
- [License](#license)

## Introduction

Financial markets are influenced by a multitude of factors, making them challenging to predict accurately. This project leverages machine learning techniques to forecast financial market trends and stock prices based on historical data. Three primary models are explored: Random Forest Regressor, ARIMA (AutoRegressive Integrated Moving Average), and Linear Regression.

## Project Overview

- `data_sources.md`: Information about the data source and data preprocessing.
- `model_explanation.md`: Explanation of selected machine learning models.
- `results/evaluation_metrics.md`: Summary of model performance metrics.
- `results/model_visualizations/`: Visualizations of model predictions.
- `usage/usage_instructions.md`: Instructions on using the project code.

## Getting Started

Follow these steps to set up the project on your local machine.

### Prerequisites

- Python 3.7 or higher
- pip package manager

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/Akshay-Sisodia/financial-predictive-analytics.git
   ```

2. Navigate to the project directory:

   ```bash
   cd financial-predictive-analytics
   ```

3. (Optional) Create a virtual environment:

   ```bash
   python -m venv venv
   ```

4. (Optional) Activate the virtual environment:

   On Windows:

   ```bash
   venv\Scripts\activate
   ```

   On macOS and Linux:

   ```bash
   source venv/bin/activate
   ```

5. Install required packages:

   ```bash
   pip install -r requirements.txt
   ```

## Data Sources

The historical data of INFY was obtained from Yahoo Finance. Refer to [data_sources.md](documentation/data_sources.md) for more details.

## Model Explanation

- Model: Random Forest Regressor
  - Description: The Random Forest Regressor is an ensemble learning technique known for its ability to handle complex relationships in financial data.
  - Parameters:
    - Number of Estimators: 200
    - Maximum Depth: 10
    - Minimum Samples Leaf: 4
    - Minimum Samples Split: 4
  - Training Process: The data is split into 3 sets
    - Training Set -70%
    - Testing Set -15%
    - Validation Set -15%
  - Model Performance:
    - Mean Squared Error (MSE): 0.04125697615099299
    - Mean Absolute Error (MAE): 0.13171805812148124
    - Root Mean Squared Error (RMSE): 0.2031181334863852
    - R-squared (R2) Score: 0.9985381695437036

## Model Performance

Refer to [evaluation_metrics.md](results/evaluation_metrics.md) for a summary of model performance metrics.

## Usage Instructions

- Preprocessing: Run `preprocessing.ipynb` to preprocess raw financial data.
- Model Training: Train the predictive models using `model_training.ipynb`.
- Model Evaluation: Evaluate model performance with `model_evaluation.ipynb`.
- Customization: Customize and extend the project as needed. Document your changes.

Refer to [usage_instructions.md](usage/usage_instructions.md) for detailed usage instructions.

## Contributing

Contributions to this project are welcome! If you have ideas for improvements or bug fixes, please open an issue or submit a pull request.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
