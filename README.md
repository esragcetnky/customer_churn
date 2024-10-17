# Classification with XGBoost and Feature Engineering through Clustering

This project addresses a binary classification problem with imbalanced classes. The dataset was analyzed and modeled using XGBoost, with additional feature engineering through clustering to enhance model performance.

## Dataset Description

The dataset contains two classes with a notable imbalance. The primary goal is to predict the correct class labels, despite the imbalance, by leveraging advanced techniques such as XGBoost and clustering for feature enhancement.

- **Input Features**: The dataset consists of multiple features (both categorical and numerical) that were used as inputs to the model.
- **Output Class**: The target variable represents two imbalanced classes, which required special handling to improve the model's predictive accuracy.

## Approach

### 1. Handling Class Imbalance
Given the imbalance between the two classes, specific techniques were used to counteract its effects:
- **Class Weighting**: Adjusting the weights during model training to give more importance to the minority class.
- **Evaluation Metrics**: Accuracy alone is not sufficient for imbalanced data. Metrics like Precision, Recall, F1-Score, and AUC-ROC were prioritized.

### 2. XGBoost Model
XGBoost was selected due to its high performance and ability to handle imbalanced datasets effectively. Key features include:
- **Boosting**: XGBoost employs gradient boosting to minimize errors iteratively.
- **Hyperparameter Tuning**: A grid search was conducted to find the best parameters for learning rate, max depth, number of estimators, and more.

### 3. Feature Engineering with Clustering
To improve the predictive power, I added a new feature created using a clustering algorithm:
- **Clustering Algorithm**: K-Means was applied to group data points based on similarity.
- **New Feature**: The cluster labels were added to the dataset as a new feature, providing the model with additional information about underlying patterns in the data.

## How to Run

1. Clone the repository:

    ```bash
    git clone https://github.com/your_username/your_repo_name.git
    cd your_repo_name
    ```

2. Install the required packages:

    ```bash
    pip install -r requirements.txt
    ```

3. Run the notebook or Python scripts to train and evaluate the model.

## Results

The XGBoost model was evaluated using the following metrics:
- **Accuracy**: Despite the imbalance, the accuracy remained competitive.
- **F1-Score**: F1 metric provided a more nuanced understanding of the model's performance on the minority class.

The addition of the clustering feature provided noticeable improvements in some evaluation metrics, especially for the minority class.

# Contact
For any questions or suggestions, feel free to reach out:

- Email: esragcetinkaya@gmail.com
- Linkedin: [esragcetinkaya](https://www.linkedin.com/in/esra-gul-cetinkaya/?locale=en_US)
