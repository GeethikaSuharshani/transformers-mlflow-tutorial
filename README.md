# 🧠 Transformers and MLflow: Downstream Tasks & Experiment Tracking

This repository demonstrates the use of pretrained transformer models for multiple NLP downstream tasks, along with systematic experiment tracking using MLflow.

---

## 🚀 Objectives

- Apply pretrained transformer models to real-world NLP tasks  
- Perform inference using Hugging Face pipelines  
- Track experiments, parameters, and outputs using MLflow  
- Compare model behavior under different conditions  

---

## 📌 Tasks Implemented

### 1. Sentiment Analysis

- Model: distilbert-base-uncased-finetuned-sst-2-english  
- Evaluated on custom sentences  
- Compared performance on normal vs sarcastic text  
- Metric: Accuracy  

---

### 2. Named Entity Recognition (NER)

- Model: dslim/bert-base-NER  
- Applied on paragraph-level inputs  
- Extracted entity types: PERSON, ORGANIZATION, LOCATION  
- Compared results on simple vs complex text  

---

### 3. Text Generation

- Model: gpt2  
- Generated text from multiple prompts  
- Compared outputs using different parameters (temperature, max_length)  

---

## 📊 Experiment Tracking with MLflow

For each task:

- Parameters (model, dataset type, generation settings) were logged  
- Metrics (accuracy, entity counts) were recorded  
- Outputs were saved as artifacts (CSV files)  
- Multiple runs were compared using MLflow UI  

---

## 📁 Repository Structure

```text
transformers-mlflow-nlp/
│
├── notebook/
│   └── transformers_mlflow.ipynb
│
├── Task_1_Sentiment_Analysis/
├── Task_2_NER/
├── Task_3_Text_Generation/
│
└── README.md
```

---

## 📌 Key Insights

- Transformer models perform well on structured inputs but struggle with nuanced language such as sarcasm
- NER performance varies with text complexity and contextual ambiguity
- Text generation quality is highly dependent on parameters such as temperature and max_length

---

## 🛠️ Technologies Used

- Python
- Hugging Face Transformers
- MLflow
- Scikit-learn
- Pandas

---

## 📎 Deliverables

- Jupyter Notebook (code + observations)
- MLflow experiment screenshots (minimum 2 runs per task)
- PDF export of notebook with analysis and observations

---