# RNA-seq Based Machine Learning for PTSD Classification

## Project Description  
This project implements a machine learning pipeline to classify **Post-Traumatic Stress Disorder (PTSD) vs. control samples** using **RNA-seq gene expression data**.  
The dataset consists of **16,231 filtered genes** (features) across **324 human blood samples**, sourced from the **GEO dataset [GSE97356]**.

### Key Steps
- **Preprocessing**: Low-expression gene filtering, normalization, and scaling  
- **Stratified Data Splitting**: Maintains class balance between PTSD and controls  
- **Modeling**: Support Vector Machine (SVM) with cross-validation and hyperparameter tuning  
- **Evaluation**: Confusion matrix, classification report, cross-validation metrics (accuracy, precision, recall, F1, ROC-AUC)  

### Results
- Test set accuracy: **~65–70%**  
- ROC-AUC: **~0.55** (indicating a modest but meaningful signal in a high-dimensional dataset)  

---

## Dataset
- **Source**: Gene Expression Omnibus (GEO) – **GSE97356**  
- **Samples**: 324 (201 controls, 123 PTSD cases)  
- **Features**: ~25,830 raw genes → 16,231 after filtering low-expression genes  

---

## Methods
- **Programming Language**: Python  
- **Libraries**: pandas, scikit-learn, numpy  
- **Machine Learning**: Support Vector Machines (SVM)  
- **Hyperparameter Optimization**: GridSearchCV  
- **Validation**: 5-fold cross-validation  

---

## Outcomes
- Identified feasibility of classifying PTSD from whole-blood RNA-seq data  
- Demonstrated an **end-to-end pipeline**: preprocessing → ML modeling → evaluation  
- Results highlight challenges in **high-dimensional, small-sample transcriptomic data** but provide a foundation for **biomarker discovery**  
