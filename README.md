# Canadian Cheese Fat Level Classification

This repository presents a machine learning classification project that predicts the fat level ("higher fat" or "lower fat") of various Canadian cheeses. The dataset was sourced from the Government of Canada's Open Data Portal.

## Objective
To classify cheese fat levels using features like moisture percentage, manufacturer details, milk treatment types, organic status, and cheese category.

## Dataset Description
The dataset includes the following columns:

- **ManufacturerProvCode:** Province code of the manufacturer
- **ManufacturingTypeEn:** Type of cheese production (Industrial/Artisan)
- **MoisturePercent:** Moisture content of the cheese
- **Organic:** Whether the cheese is organic (binary)
- **CategoryTypeEn:** Category of cheese (Firm, Semi-soft, Fresh Cheese, etc.)
- **MilkTypeEn:** Type of milk used (Cow, Goat, etc.)
- **MilkTreatmentTypeEn:** Treatment type of milk (Pasteurized, Raw, etc.)
- **CheeseName:** Name of the cheese
- **FatLevel (Target):** Fat classification (higher fat/lower fat)

## Methodology
The following approaches were used:

- **Data Preprocessing:** Handled missing values, encoding of categorical data, and text vectorization.
- **Baseline Model:** Dummy classifier for initial comparison.
- **Advanced Models:** Support Vector Classifier (SVC) and K-Nearest Neighbors (KNN), including hyperparameter tuning and cross-validation.
- **Evaluation Metrics:** Precision, Recall, F1-score, and Accuracy.

## Technologies Used
- Python
- Pandas, NumPy
- Scikit-learn (Pipeline, OneHotEncoder, CountVectorizer, SimpleImputer, KNN, SVC)
- Matplotlib, Seaborn for data visualization
- Altair for advanced visualizations

## Results
- The best performing model was **Support Vector Classifier (SVC)** with hyperparameter tuning:
  - Accuracy: **87%**
  - F1-score: **90%**

- KNN (after tuning) achieved an accuracy of **84%**, while the baseline Dummy Classifier had **65%** accuracy.
