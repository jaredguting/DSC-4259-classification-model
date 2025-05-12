# Intelligent Systems - DSC 4156
**Course:** Intelligent Systems 

## Overview  
This project explores the classification of crime incidents in Los Angeles using machine learning and reinforcement learning techniques. The goal is to predict the crime code (`Crm Cd`) based on various encoded features such as location, victim demographics, and time of occurrence.

### Models Implemented:
- **Deep Q-Network (DQN)** – a reinforcement learning-based classifier  
- **XGBoost Classifier** – a gradient boosting algorithm optimized for performance

### Additional Highlights:
- Class imbalance handling using SMOTE.
- Feature engineering for temporal and demographic patterns.
- Interpretability with **SHAP** and **LIME**.
- Bootstrapped confidence intervals for F1 scores.
## Limitations  

- The Deep Q-Network (DQN) performed poorly due to the static nature of the classification task, which is not ideal for reinforcement learning.  
- The dataset is highly imbalanced, with over 100 crime classes, many of which have very few samples.  
- Even with XGBoost and SMOTE, rare classes remain difficult to classify accurately.  
- Feature interpretability can vary depending on the model, and explanations are less reliable for underrepresented classes.  

---

## Notes  

- The original dataset contains over 1 million records. A subset of 250,000 rows was used due to computational constraints.  
- Crime codes (`Crm Cd`) are treated as categorical labels in a multi-class classification setting.  
- Class filtering was applied to remove very rare labels with fewer than 4 instances before training.  
- Evaluation was performed using both macro and weighted metrics to account for class imbalance.  

---

## Disclaimer  

This project is intended for submission purposes only.  
The dataset is publicly available and has been used here to demonstrate machine learning techniques.  
No conclusions from this project should be used in actual law enforcement, policymaking, or public safety decisions.  
Always adhere to ethical guidelines and consult domain experts when working with sensitive or real-world data.
