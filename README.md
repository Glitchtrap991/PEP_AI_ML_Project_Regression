# 📈 PEP AI/ML Project: Student Score Predictor

## 🧠 Project Overview
This project implements **Simple Linear Regression (SLR)** to analyze and predict student exam scores based on the number of hours they dedicated to studying.

The goal is to model the linear relationship between these two variables, providing insight into the correlation between effort (study hours) and outcome (exam score).

## 🛠️ Model Details
The model calculates the coefficients for the equation of a straight line:

$$
\text{Score} = m \times \text{Hours} + c
$$

* **Independent Variable ($X$):** Hours Studied
* **Dependent Variable ($y$):** Exam Score
* **Model:** `sklearn.linear_model.LinearRegression`

## 🚀 Getting Started

Follow these steps to clone the repository and run the analysis locally.

### Prerequisites

You must have Python installed. The required libraries are listed in `requirements.txt`.

1.  **Clone the Repository:**
    ```bash
    git clone [https://github.com/Glitchtrap991/PEP_AI_ML_Project_Regression.git](https://github.com/Glitchtrap991/PEP_AI_ML_Project_Regression.git)
    cd PEP_AI_ML_Project_Regression
    ```

2.  **Create a Virtual Environment (Recommended):**
    ```bash
    python -m venv venv
    source venv/bin/activate  # On Windows, use 'venv\Scripts\activate'
    ```

3.  **Install Dependencies:**
    ```bash
    pip install -r requirements.txt
    ```

4.  **Run the Notebook:**
    Open the `Student_Score_Predictor.ipynb` file in Google Colab, Jupyter Notebook, or VS Code to run the steps, train the model, and view the results.

## 📊 Results and Evaluation

### Line of Best Fit
The model output shows the calculated coefficients:

| Coefficient | Value | Interpretation |
| :--- | :--- | :--- |
| **Slope ($m$)** | 5.87 | Score increase per one extra hour of study. |
| **Intercept ($c$)**|39.02 | Predicted score for 0 hours of study. |

### Performance Metrics
The model was evaluated using the Mean Absolute Error (MAE):

* **Mean Absolute Error (MAE):** 10.84 - _*This means the model's predictions are, on average, off by this many points.*_
* **Mean Squared Error (MAE):** 170.09 - _*Calculates the average of the squared errors. Because errors are squared, this metric gives disproportionately high weight to large errors (outliers), making it useful for optimizing the model. *_
* **R-Squared (R2) :** 0.52 - _**Goodness of Fit:** Represents the proportion of the variance in the dependent variable (Score) that is predictable from the independent variable (Hours Studied). The value ranges from 0 to 1, where a value closer to 1 indicates a better fit._

### Visual Output
(Optional: Include a link to an image of your scatter plot with the regression line for visual impact!)

## 🔮 Sample Prediction

Using the trained model, if a student studies for **9.25 hours**:
* **Predicted Score:** 91.82

---

## ✍️ Author

* Glitchtrap991
