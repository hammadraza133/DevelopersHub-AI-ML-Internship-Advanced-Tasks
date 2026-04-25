# AI/ML Engineering Advanced Internship - Task Portfolio
**Developer:** Muhammad Hammad Raza 
**Organization:** DevelopersHub Corporation  
**Project Duration:** 2026

---

## 📌 Overview
This repository contains a series of advanced Machine Learning and Deep Learning projects completed during the AI/ML Engineering Advanced Internship. The tasks span Natural Language Processing (NLP), Production ML Pipelines, and Multimodal Deep Learning.

---

## 🚀 Tasks Summary

### Task 1: News Topic Classifier Using BERT
Fine-tuned a **BERT transformer model** (`bert-base-uncased`) to classify news headlines into four categories: World, Sports, Business, and Sci/Tech.

* **Approach**: Tokenized text using `BertTokenizerFast` and fine-tuned using the Hugging Face `Trainer` API.
* **Performance**: Achieved approximately 93–95% Accuracy and Macro F1-score.
* **Deployment**: Implemented a real-time web interface using **Gradio** and a standalone **Streamlit** application.

### Task 2: End-to-End Churn Prediction Pipeline
Developed a production-ready ML pipeline to predict customer churn using the Telco Customer Churn Dataset.

* **Approach**: Built a `ColumnTransformer` for automated preprocessing (StandardScaler for numerical data, OneHotEncoder for categorical) and used `GridSearchCV` for hyperparameter tuning.
* **Performance**: Random Forest outperformed Logistic Regression with an **ROC-AUC of ~0.86**.
* **Key Insight**: Tenure and Contract Type were identified as the strongest predictors of churn.

### Task 3: Multimodal Housing Price Prediction
Built a deep learning architecture to predict housing prices by fusing **tabular features** with **visual data** extracted from images.

* **Approach**: Used **MobileNetV2** (transfer learning) to extract features from house images and a Dense Neural Network for tabular data.
* **Fusion**: Combined both modalities via a concatenation layer to perform final price regression.
* **Performance**: The multimodal model showed a significant improvement in Mean Absolute Error (MAE) compared to a tabular-only baseline.

---

## 🛠️ Technology Stack
* **Deep Learning**: TensorFlow, Keras, PyTorch, Hugging Face Transformers.
* **Machine Learning**: Scikit-learn (Pipelines, GridSearchCV).
* **Data Science**: Pandas, NumPy, Matplotlib, Seaborn.
* **Deployment**: Gradio, Streamlit.
* **Serialization**: Joblib.

---

## 📂 Repository Structure
```bash
.
├── Task 1.ipynb                 # News Classification (BERT)
├── Task 2.ipynb                 # Churn Prediction Pipeline
├── Task 3.ipynb                 # Multimodal Housing Prediction
├── app_task1.py                 # Streamlit App for News Classifier
├── churn_pipeline_rf.joblib     # Exported Production Pipeline
└── README.md                    # Project Documentation

