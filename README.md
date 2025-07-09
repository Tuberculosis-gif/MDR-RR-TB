# MDR/RR-TB Treatment Outcome Prediction Model

## 📌 Overview
This project develops machine learning models to **predict culture conversion outcomes at 2/6 months** for multidrug-resistant/rifampicin-resistant tuberculosis (MDR/RR-TB) patients. The goal is to enable early intervention and improve clinical decision-making for this high-risk population.

## 🔍 Research Background
Early prediction of MDR/RR-TB treatment outcomes is critical for:
- Improving patient survival rates  
- Reducing disease transmission  
- Optimizing resource allocation in TB control programs  

## 🎯 Objectives
1. Build predictive models using **logistic regression** and **7 ML algorithms**  
2. Compare performance to identify the optimal model  
3. Validate generalizability via external clinical cohorts  
4. Provide a tool for early therapy efficacy assessment  

## ⚙️ Methodology
### Data Sources
| Cohort        | Period          | Patients | Usage        |
|---------------|-----------------|----------|--------------|
| Hospital 1    | Jan 2017–Jun 2023 | 744      | Training Set |
| Hospital 2    | Mar 2021–Jun 2022 | 137      | Validation Set |

### Models Developed
- **Single Models**:
  - Logistic Regression (LR)
  - Random Forest (RF)
  - Support Vector Machine (SVM)
  - Gradient Boosting Decision Tree (GBDT)
  - Elastic Net (EN)
  - Artificial Neural Network (ANN)
- **Ensemble Methods**:  
  - Stacking (using RF, SVM, GBDT, EN, ANN as base learners)
  - Voting (using RF, SVM, GBDT, EN, ANN as base learners)

### Evaluation Metrics
- AUC (Area Under ROC Curve)  
- Accuracy  
- Sensitivity  
- Specificity  

## 📊 Key Results
**Optimal Model**: Artificial Neural Network (ANN)  

**Training Performance**:
| Timepoint | AUC (95% CI)       | Accuracy | Sensitivity | Specificity |
|-----------|--------------------|----------|-------------|-------------|
| 2-month   | 0.82 (0.77–0.86)  | 0.74     | 0.74        | 0.75        |
| 6-month   | 0.90 (0.86–0.93)  | 0.80     | 0.79        | 0.87        |

**Validation Performance**:
| Timepoint | AUC (95% CI)       |
|-----------|--------------------|
| 2-month   | 0.86 (0.76–0.93)  |
| 6-month   | 0.74 (0.61–0.88)  |

## 💡 Conclusion
- ANN provides **superior accuracy** in predicting early culture conversion compared to other models.  
- ML models show **better stability and generalizability** than logistic regression.  
- This tool enables rapid identification of high-risk patients for personalized therapy adjustment.  

## 🚀 Application Value
- Supports clinical decision-making for MDR/RR-TB management  
- Facilitates resource prioritization in TB control programs  
- Provides a framework for extending predictive modeling to other drug-resistant infections  

---
