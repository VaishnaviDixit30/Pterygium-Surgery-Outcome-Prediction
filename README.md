# Pterygium Surgery Outcome Prediction using Deep Learning

This project focuses on developing **Deep Learning–based predictive models** to estimate both **post-operative clinical outcomes** and **surgical complications** following **pterygium surgery**. Predictions are generated for **7-day and 30-day follow-up periods**, supporting early risk assessment and informed post-surgical decision-making.

By integrating clinically meaningful ophthalmic parameters with modern neural network architectures, this project demonstrates how data-driven systems can assist ophthalmologists in anticipating recovery trends and potential complications.

---

## Project Objectives

- **Realistic Clinical Data Simulation**  
  Generate a comprehensive synthetic dataset that closely reflects real-world pterygium surgery cases, including patient demographics, pre-operative measurements, and post-operative follow-up outcomes.

- **Data Preparation for Machine Learning**  
  Clean, encode, and standardize all categorical and numerical clinical features (such as gender, residential area, and affected eye) to ensure compatibility with Deep Learning models.

- **Clinical Outcome Prediction (Regression)**  
  Train a Deep Learning regression model to predict **8 continuous clinical parameters**—including visual acuity, refractive values, and keratometry readings—at **30 days post-surgery**.

- **Post-Surgical Complication Prediction (Classification)**  
  Develop a multi-output classification model to predict the **occurrence and type of complications** at both **7-day and 30-day post-operative follow-ups**.

---

## Project Structure

| File Name | Description |
|----------|-------------|
| `Data_generation.ipynb` | Generates a clinically realistic **synthetic dataset** of 350 patient records, simulating demographics, pre-operative findings, and post-operative outcomes. |
| `Data_Preprocessing.ipynb` | Cleans the dataset and converts categorical variables into numerical form using **Label Encoding**, preparing the data for model training. |
| `Model_training.ipynb` | Trains and evaluates two Deep Learning models: a **regression model** for clinical outcome prediction and a **multi-output classification model** for complication prediction. |
| `README.md` | Provides an overview of the project’s scope, methodology, and outputs. |

---

## Generated Outputs

- `original_data.csv`  
  Raw synthetic dataset containing patient demographics and clinical variables.

- `prep_data.csv`  
  Preprocessed dataset formatted for Deep Learning workflows.

- `regression_model.h5`  
  Saved Keras model for predicting 30-day continuous clinical outcomes.

- `classification_model.h5`  
  Saved Keras model for predicting post-surgical complications at 7-day and 30-day intervals.

---

## Significance of the Project

Pterygium is a prevalent ocular condition, especially in regions with high ultraviolet exposure. Accurate prediction of surgical outcomes and potential complications can:

- Improve post-operative care planning  
- Assist ophthalmologists in clinical decision-making  
- Highlight the practical application of Deep Learning in healthcare analytics  

This project serves as a strong example of how **artificial intelligence can complement clinical expertise**, making it suitable for academic research, healthcare-focused hackathons, and professional AI/ML portfolios.

---
