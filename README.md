 # Customer Churn Prediction

#  Project Overview
This project aims to **predict customer churn** using a **Neural Network** built with **Keras/TensorFlow**.  
The data is **one-hot encoded**, followed by **exploratory data analysis** and **deep learning model training**.


#  Data Preprocessing
- **One-hot encoding** applied to all categorical variables.
- Scaled numerical columns using StandardScaler.
-  Split into training and testing sets with stratify=y to preserve class balance.



# Exploratory Data Analysis (EDA)
-  **Univariate Analysis**: Distribution of individual features (e.g. churn rate, tenure, monthly charges).  
-  **Bivariate Analysis**: Relationships between categorical features (e.g. contract type vs churn) displayed using stacked and grouped bar plots.  
-  **Multivariate Analysis**:
  - Pair plots of key numeric features colored by `Churn`.
  - Correlation heatmaps to understand feature relationships.
  - Facet grids for deeper feature interactions.

---

##  Model Architecture
Built a **Sequential Neural Network** with:
-  **Dense layers** with relu activation.
-  **Output layer** with a single unit and sigmoid activation.
-  Trained for **160 epochs** with **EarlyStopping** and **ReduceLROnPlateau** callbacks.
-  **Adam optimizer** with binary_crossentropy loss.
-  Metrics: Precision, Recall, AUC, and Accuracy.



##  Model Performance
-  **Accuracy**: 0.716  
-  **AUC**: 0.86  
-  Balanced evaluation on precision and recall to account for class imbalance.


##  Future Improvements
This is a **work-in-progress** — further optimization is planned:
-  Experimenting with **hyperparameter tuning** (layer sizes, learning rates, regularization).
-  Addressing class imbalance using techniques like **SMOTE** or **class weights**.
- Exploring **alternative models** (Random Forest, XGBoost) for better baseline comparisons.



