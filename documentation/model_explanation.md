## Model explanation: Random Forest Regressor

- **Description**: The Random Forest Regressor is an ensemble learning technique that combines multiple decision trees to make predictions. It is well-suited for regression tasks and is known for its ability to handle complex relationships in the data.

- **Parameters**: The key hyperparameters and their values for the Random Forest Regressor used in this project are as follows:
  - Number of Estimators: 200
  - Maximum Depth: 10
  - Minimum Samples Leaf: 4
  - Minimum Samples Split: 4

- **Training Process**: The model was trained using the following steps:
  - Data was split into training and validation sets (70% training, 30% validation).
  - The Random Forest Regressor was initialized with the specified hyperparameters.
  - The model was trained on the training data.
  - Cross-validation techniques were not applied in this case.

- **Model Performance**: The Random Forest Regressor's performance on the validation set was evaluated using the following metrics:
  - Mean Squared Error (MSE): 0.04125697615099299
  - Mean Absolute Error (MAE): 0.13171805812148124
  - Root Mean Squared Error (RMSE): 0.2031181334863852
  - R-squared (R2) Score: 0.9985381695437036

## Model Selection Rationale

- **Explanation**: The models were selected based on their suitability for financial predictive analytics. The Random Forest Regressor was chosen because it is known for its robustness and ability to capture complex patterns in financial data.