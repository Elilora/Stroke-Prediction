# **Stroke Prediction Model**

This project aims to predict the likelihood of a stroke using various machine learning models based on the `healthcare-dataset-stroke-data.csv` dataset. The dataset contains information on various health attributes that may contribute to stroke occurrence.

## **Table of Contents**

- [Installation](#installation)
- [Usage](#usage)
- [Dataset](#dataset)
- [Data Preprocessing](#data-preprocessing)
- [Model Building](#model-building)
- [Results](#results)
- [Contributing](#contributing)
- [License](#license)

## **Installation**

1. **Clone the repository:**

    ```bash
    git clone https://github.com/yourusername/stroke-prediction.git
    cd stroke-prediction
    ```

2. **Install the required libraries:**

    ```bash
    pip install numpy pandas seaborn matplotlib scikit-learn xgboost shap
    ```

## **Usage**

1. **Ensure the dataset file `healthcare-dataset-stroke-data.csv` is in the `/kaggle/input/stroke-prediction-dataset/` directory.**

2. **Run the script to train and evaluate the models:**

    ```bash
    python stroke_prediction.py
    ```

## **Dataset**

The dataset used for this project is `healthcare-dataset-stroke-data.csv`, which contains the following columns:

- `id`
- `gender`
- `age`
- `hypertension`
- `heart_disease`
- `ever_married`
- `work_type`
- `Residence_type`
- `avg_glucose_level`
- `bmi`
- `smoking_status`
- `stroke`

## **Data Preprocessing**

1. **Handle missing values:**
    - The `bmi` column had missing values, which were imputed using the mean strategy.
2. **Encode categorical variables:**
    - Categorical columns were encoded using `LabelEncoder`.

## **Model Building**

The following models were used to predict stroke occurrence:

- Decision Tree Classifier
- Random Forest Classifier

### **Steps**

1. **Split the data into training and testing sets (70% train, 30% test).**
2. **Train the models on the training set.**
3. **Evaluate the models on the testing set using accuracy and F1-score metrics.**
4. **Generate classification reports and confusion matrices.**

## **Results**

### **Decision Tree Classifier**

- **Accuracy:** 91.06%
- **F1-score:** 10.46%
- **Detailed classification report and confusion matrix are generated in the script output.**

### **Random Forest Classifier**

- **Accuracy:** 95.50%
- **F1-score:** 0.00%
- **Detailed classification report and confusion matrix are generated in the script output.**

## **Contributing**

Contributions are welcome! Please fork the repository and submit a pull request for any enhancements or bug fixes.

## **License**

This project is licensed under the MIT License - see the LICENSE file for details.
