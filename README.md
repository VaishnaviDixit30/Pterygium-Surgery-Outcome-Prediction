# Pterygium-Surgery-Outcome-Prediction

The core objective of this project is to build Deep Learning models that predict the clinical and complication outcomes of Pterygium surgery at 7-day and 30-day post-operative follow-ups.

## Overall Code Objective

* **Simulate Realistic Clinical Data:** The project creates a detailed, synthetic dataset for patient records related to pterygium surgery .
* **Prepare Data for ML:** Clean and encode categorical features (like `gender`, `area`, `affected_eye`) to make the data suitable for model input.
* **Predict Clinical Outcomes:** Use a Deep Learning Regression Model to forecast 8 continuous metrics (vision, refraction, keratometry) 30 days post-surgery.
* **Predict Complications:** Use a Deep Learning Classification Model to predict the likelihood and type of complications at both 7 and 30 days post-surgery.

## Project Files Description

| File Name | Description |
| :--- | :--- |
| `Data_generation.ipynb` | This notebook uses Python to create a **synthetic dataset** of 350 patient records. It simulates patient demographics, pre-operative clinical metrics, and two post-operative follow-up results (7 days and 30 days) . |
| `Data_Preprocessing.ipynb` | This script takes the generated data and prepares it for machine learning . It converts all non-numerical categories (like gender and location) into numerical labels using a **LabelEncoder** . |
| `Model_training.ipynb` | This is where the two **Deep Learning models** are trained and evaluated .It trains a **regression model** for clinical outcomes and a **multi-output classification model** for complications. |
| `README.md` | The overview file you are currently reading. |

## Model Outputs (Generated Files)

* `original_data.csv`: The initial raw, synthetic dataset.
* `prep_data.csv`: The preprocessed dataset ready for model training.
* `regression_model.h5`: Saved Keras model for predicting 30-day continuous clinical outcomes.
* `classification_model.h5`: Saved Keras model for predicting 7-day and 30-day complications.
