# AI-Research-Project
Final Project for Sheridan AI course 2025 


# 🍷 Wine Quality Classification — Red Wine (Machine Learning Project)

This repository contains my final project for the Wine Quality Classification task using the **Red Wine Quality Dataset** from the UCI Machine Learning Repository. The goal of the project was to predict wine quality based on various physicochemical attributes using machine learning models, implemented through the PyCaret classification framework.

---

## 📄 Abstract

In this project, I used the Red Wine Quality dataset from the UCI Machine Learning Repository to predict wine quality based on different chemical measurements. I treated the quality score as a classification problem and used PyCaret to test and compare multiple machine learning models. After running the comparisons, the **Extra Trees Classifier** turned out to be the best model, reaching about **70% accuracy** and around a **0.68 F1-score**. I also tried tuning the model, but the tuned version didn’t improve, so the original model was kept as the final choice. The evaluation results showed that the model performs well on the common quality classes and struggles with the rarer ones, which makes sense given the imbalance in the dataset. The feature importance analysis also lined up with real wine chemistry—for example, alcohol and sulphates were among the top predictors. Overall, the project showed that tree-based ensemble models work well for this dataset and that PyCaret makes it much easier to build, test, and evaluate several models quickly.

---

## 🎥 Video Presentation

You can watch my short 5-minute presentation here:

👉 **YouTube Link:** https://youtu.be/fNE_I1uypYs

---

## 📁 Files in This Repository

- **wine_quality_project_full.ipynb** — Full Jupyter Notebook with EDA, model comparison, tuning, and evaluation  
- **README.md** — This file  

(If needed, add your dataset locally when running the notebook — it is not uploaded here because the assignment states to only include the notebook.)

---

## 🧪 Project Summary

- **Dataset:** Red Wine Quality (UCI)
- **Task:** Multiclass classification  
- **Target:** `quality` (converted to categorical)  
- **Models Tested:** Logistic Regression, Random Forest, Extra Trees, XGBoost, LightGBM, CatBoost, etc.  
- **Best Model:** **Extra Trees Classifier**  
- **Best Performance:**  
  - Accuracy ≈ **0.70**  
  - F1-score ≈ **0.68**  
  - Micro-AUC ≈ **0.93**

---

## ⚙️ Environment & Tools

This project was built using:

- Python 3.11  
- PyCaret 3.3.2  
- pandas 2.1.4  
- numpy 1.26.4  
- scikit-learn (via PyCaret)  
- Google Colab (Runtime: 2025.07)

---

## 🚀 How to Run the Notebook

1. Download the notebook:  
   `FinalAI_YoussefA.ipynb`

2. Get the dataset (`winequality-red.csv`) from the UCI Machine Learning Repository.

3. Open the notebook in **Google Colab** or Jupyter.

4. Upload the dataset when prompted in the notebook:

```python
from google.colab import files
files.upload()
